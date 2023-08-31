<script>
	import Link from '../../lib/components/Link.svelte';
</script>

<svelte:head>
	<title>Hisam Fahri</title>
</svelte:head>


<div class="flex flex-row items-center justify-start space-x-4 mt-24">
	<div>
		<h2 class="text-lg font-semibold">Journals</h2>
    <a class="text-base font-normal text-gray-400" href="/">Home</a>
	</div>
</div>

<div class="mt-8">
	<p class="text-sm text-gray-700">My thougths, my perspective, and my wildest ideas.</p>
</div>

<div class="mt-8">
	<Link
		name="2023-08-24"
		href="/journals/2023-08-24"
		display="The Case Against Specialists (and Generalists)"
	/>
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
