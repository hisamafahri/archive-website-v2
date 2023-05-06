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
		<p class="text-base font-normal text-gray-400">Software Engineer</p>
	</div>
</div>

<div class="mt-8">
	<p class="text-sm text-gray-700">
		I'm an engineer interested in system and design architecture (well technically every part of
		building a product)
	</p>
</div>

<div class="mt-8">
	<h3 class="mb-6 font-semibold">Links</h3>
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

<div class="mt-8">
	<h3 class="mb-6 font-semibold">Projects</h3>
	<Link
		name="ngoding.org"
		href="https://ngoding.org"
		target="_blank"
		display="Learn to code, for free, for everyone"
	/>
	<Link
		name="codefly"
		href="https://github.com/hisamafahri/codefly"
		target="_blank"
		display="Share your code snippets anonimously"
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
		display="(WIP) My own programming language (I guess?)"
	/>
	<div class="mt-8 w-min">
		<a
			class="text-sm text-gray-700 hover:underline whitespace-nowrap no-underline"
			target="_blank"
			href="https://github.com/hisamafahri"><p>And much more...</p></a
		>
	</div>
</div>

<div class="mt-8 mb-24">
	<h3 class="mb-6 font-semibold">Journals</h3>
	<Link
		name="2023-04-24"
		href="/journals/2023-04-24"
		display="Rule #0 for Product Managers"
	/>
	<Link
		name="2023-03-12"
		href="/journals/2023-03-12"
		display="Building a Product? Always Strive for the 'Right' Execution"
	/>
	<Link
		name="2023-02-20"
		href="/journals/2023-02-20"
		display="Personalised Development Environment"
	/>
	<Link
		name="2023-02-03"
		href="/journals/2023-02-03"
		display="Declared vs Inferred Types, a Debate of the Century"
	/>
	<Link name="2023-01-29" href="/journals/2023-01-29" display="Hello, world!" />
</div>
