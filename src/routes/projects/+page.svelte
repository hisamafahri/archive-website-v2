<script>
	import Link from '../../lib/components/Link.svelte';
</script>

<svelte:head>
	<title>Hisam Fahri</title>
</svelte:head>

<div class="flex flex-row items-center justify-start space-x-4 mt-24">
	<div>
		<h2 class="text-lg font-semibold">Projects</h2>
		<a class="text-base font-normal text-gray-400" href="/">Home</a>
	</div>
</div>

<div class="mt-8">
	<p class="text-sm text-gray-700">
		Lately, a lot of my projects (or wannabe startups you might call them) are
		in a private repositories. But, here are some notable open-source projects
		of mine:
	</p>
</div>

<div class="mt-8">
	<Link
		name="ngoding.org"
		href="https://ngodingorg.vercel.app"
		target="_blank"
		display="Learn to code, for free, for everyone"
	/>
	<Link
		name="MyPocket"
		href="https://github.com/hisamafahri/mypocket"
		target="_blank"
		display="Pocket, but far more better!"
	/>
	<Link
		name="codefly"
		href="https://github.com/hisamafahri/codefly"
		target="_blank"
		display="Share your code snippets anonymously"
	/>
	<Link
		name="samstack"
		href="https://github.com/hisamafahri/samstack"
		target="_blank"
		display="Bleeding edge tech stack for supa-fast development"
	/>
	<Link
		name="coco"
		href="https://github.com/hisamafahri/coco"
		target="_blank"
		display="Color converter package for Go"
	/>
	<Link
		name="nit"
		href="https://github.com/hisamafahri/nit"
		target="_blank"
		display="Git CLI wrapper to make it more fun"
	/>
	<Link
		name="create-min-app"
		href="https://github.com/hisamafahri/create-min-app"
		target="_blank"
		display="Generate minimum projects in various tech-stack, easily"
	/>
	<Link
		name="editr"
		href="https://github.com/hisamafahri/editr"
		target="_blank"
		display="Yet another simple Rich Text Editor"
	/>
	<Link
		name="tulkit"
		href="https://github.com/hisamafahri/tulkit"
		target="_blank"
		display="Rust desktop app for my daily needs"
	/>
	<Link
		name="letta"
		href="https://github.com/hisamafahri/letta"
		target="_blank"
		display="(WIP) UI library that doesn't sucks"
	/>
	<Link
		name="todomi"
		href="https://github.com/hisamafahri/todomi"
		target="_blank"
		display="(WIP) My very own programming language (I guess?)"
	/>
	<div class="mt-8 w-min">
		<a
			class="text-sm text-gray-700 hover:underline whitespace-nowrap no-underline"
			target="_blank"
			href="https://github.com/hisamafahri"><p>And much more...</p></a
		>
	</div>
</div>
