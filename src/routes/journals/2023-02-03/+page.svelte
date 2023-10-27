<script>
	import { HighlightAuto } from 'svelte-highlight';
	import github from 'svelte-highlight/styles/github';
	import typescript from 'svelte-highlight/languages/typescript';
</script>

<svelte:head>
	{@html github}
	<title
		>Declared vs Inferred Types, a Debate of the Century - Hisam's Journal</title
	>
</svelte:head>

<div class="mt-24 mb-12">
	<h1 class="text-xl font-semibold">
		Declared vs Inferred Types, a Debate of the Century
	</h1>
	<p class="text-base font-normal text-gray-400">
		2023-02-03 by <a href="/">Hisam Fahri</a>
	</p>
</div>

<div class="content">
	<h3 class="head-section">What on earth is all of this about?</h3>
	<p>
		Well, I might be exaggerating on the title. But, I think this little journal
		will get a little exciting (and a little bit spicy of course). If you've
		ever written Typescript before, you'll notice that the Typescript compiler
		is smart enought to infer types of the code you've been writing. It's surely
		really helpful, right?
	</p>

	<h3 class="head-section">A double-edged sword</h3>
	<p>Let's create a simple function for the sake of demonstration:</p>
	<br />
	<HighlightAuto
		language={typescript}
		code={`// sample.ts
function convertString(str: string) {
    return parseInt(str);
}

const result: number = convertString("1");
`}
	/>

	<br />
	<p>
		Well, everything looks fine, right? Is there a problem here? Well, yes. but
		there's a catch.
	</p>

	<h3 class="head-section">Developers are human (at least for now)</h3>
	<p>
		Developers can make mistakes. They can make a lot of mistakes. My personal
		preference is that a piece of code should (as best as possible) explain
		themselves. This often being supported by comments left by the developer
		itself, name, and the <strong>types</strong>.
	</p>
	<br />
	<p>
		Let's set an imaginary case. If your teammates (or even you) try to change
		the return of a function without checking all of the references of the
		function, this can lead to messy problems that might waste a lot of your
		time. If we take the above piece of code and directly mess around with the
		return type:
	</p>
	<br />
	<HighlightAuto
		language={typescript}
		code={`// sample.ts
function convertString(str: string) {
    return parseInt(str).toString();
}

const result: number = convertString("1");
      // ^?: Type 'string' is not assignable to type 'number'.
`}
	/>
	<br />
	<p>
		If the implementation, the function (producer) and the usage (consumer)
		itself are simple, this problem might be easy to fix. But, often time in
		real-world implementations, a real-world application, the implementation is
		astronomically more difficult than in the example above.
	</p>
	<br />
	<p>
		In the code above, you as a developer might think that your consumer is at
		fault, and spend a lot of time trying to have a lot of weird working around
		just to "make it work".
	</p>
	<br />
	<HighlightAuto
		language={typescript}
		code={`// sample.ts
const result: number = parseint(convertString("1"));
`}
	/>

	<h3 class="head-section">Just "say" it out loud</h3>
	<p>
		Some peoples might find this as a hot takes, but declaring your types (for
		input, and expected output) might be a tedious work at start, but it is
		surely worth it. Why? Let's take a look at the code again:
	</p>
	<br />
	<HighlightAuto
		language={typescript}
		code={`// sample.ts
function convertString(str: string): number {
    return parseInt(str).toString();
      // ^?: Type 'string' is not assignable to type 'number'.
}

const result: number = convertString("1");
`}
	/>
	<br />
	<p>
		As you can see, the error moves from the consumer to the producer itself.
		Because it is the producer's fault itself at faults here. The example above
		is surely an oversimplification of what actually could happen in a
		real-world application.
	</p>
	<h3 class="head-section">Read it easily</h3>
	<p>
		Not only does our function become more "secure", it also makes our function
		itself more readable. And, as I mentioned earlier, the code speaks for
		itself. Even though we name our function <code>convertString()</code>, since
		we explicitly declare refer function as a <code>number</code>, it'll
		intuitively explain that our function is converting a string to a number.
	</p>
	<h3 class="head-section">Should I declare everything then?</h3>
	<p>
		Well, finally it comes back to your use cases and preferences. Have been
		working with a lot of low-level languages made me comfortable with declaring
		types explicitly rather than relying on the compiler to do that for me.
	</p>
	<br />
	<p>
		It surely is an extra piece of code, but I felt amazing using it. In the
		end, it comes down to you to decide.
	</p>
</div>
