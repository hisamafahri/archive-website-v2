<script>
	import profile from '$lib/assets/image/profile.jpeg';
	import Link from '../lib/components/Link.svelte';
</script>

<svelte:head>
	<title>Hisam Fahri</title>
</svelte:head>

<div class="flex flex-row items-center justify-start space-x-4 mt-24">
	<img class="rounded-full w-14 h-14" src={profile} alt="profile" />
	<div>
		<h2 class="text-lg font-semibold">Hisam Fahri</h2>
		<p class="text-base font-normal text-gray-400">Reader, developer, dream catcher.</p>
	</div>
</div>

<div class="mt-8">
	<p class="text-sm text-gray-700">
		I'm an engineer that can wear many hats (well technically every hat for building a product)
	</p>
</div>

<div class="mt-8">
	<h3 class="mb-6 font-semibold">Links</h3>
	<Link
		target="_blank"
		name="Chat with Me"
		href="https://cal.com/hisam"
		display="cal.com/hisam"
	/>
	<Link
		target="_blank"
		name="GitHub"
		href="https://github.com/hisamafahri"
		display="@hisamafahri"
	/>
	<Link
		target="_blank"
		name="Twitter"
		href="https://twitter.com/hisamafahri"
		display="@hisamafahri"
	/>
	<Link
		target="_blank"
		name="LinkedIn"
		href="https://linkedin.com/in/hisamafahri"
		display="/in/hisamafahri"
	/>
	<Link
		target="_blank"
		name="Email me"
		href="mailto:me@hisamafahri.com"
		display="me@hisamafahri.com"
	/>
</div>

<div class="my-16">
	<h3 class="mb-6 font-semibold">My Craft</h3>
	<Link target=" " name="Thoughts & Ideas" href="journals" display="Journal Collections" />
	<Link target=" " name="Works" href="projects" display="Project Collections" />
</div>

<div class="my-16">
	<h3 class="mb-6 font-semibold">Some Things I Believe</h3>
	<ul class="list-disc space-y-6">
		<li>It&apos;s important to do things FAST!</li>
		<ul class="ml-6 list-[circle] !mt-1">
			<li>Time is finite resources</li>
			<li>Time is the denominator</li>
			<li>A week is 2% of the year</li>
			<li>Going fast makes you focus on what's important. No wasted time for the unimportant</li>
		</ul>
		<li>Enthusiasm and genuine curiosity matters</li>
		<ul class="ml-6 list-[circle] !mt-1">
			<li>It&apos;s so much easier working on something that exictes us</li>
			<li>It might be one of the biggest survival factor for the things that we're working on</li>
		</ul>
		<li>The red string of every problem is interpersonal relationship problems</li>
		<ul class="ml-6 list-[circle] !mt-1">
			<li>Life is not a "competition", rather than a cooperation</li>
			<li>We are the only one that worrying about our looks (and of course, our ideas)</li>
			<li>Admitting fault is not a defeat</li>
		</ul>
		<li>Smaller teams are better</li>
		<ul class="ml-6 list-[circle] !mt-1">
			<li>Faster decisions, fewer meetings, more experiments, more fun</li>
			<li>No room for mediocre people (can pay more, too!)</li>
			<li>
				Hire another peoples should be the last option (after internal implementations and third
				party services)
			</li>
		</ul>
		<li>We should build something insanely great</li>
		<ul class="ml-6 list-[circle] !mt-1">
			<li>Term "MVP" is often being abused. MVP shouldn&apos;t sacrifice quality</li>
			<li>"This is a minimal product, so quality isn't important" is a lie</li>
			<li>
				If you don’t have the expertise, resources, OR courage to build something, then don&apos;t
			</li>
		</ul>
	</ul>
</div>
