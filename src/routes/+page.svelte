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
		I'm an engineer interested in system and design architecture (well technically every part of
		building a product)
	</p>
</div>

<div class="mt-8">
	<h3 class="mb-6 font-semibold">Links</h3>
	<Link
    target=" "
		name="Thoughts & Ideas"
		href="journals"
		display="Journal Collections"
	/>
	<Link
    target=" "
		name="Works"
		href="projects"
		display="Project Collections"
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

<div class="mt-16">
	<h3 class="mb-6 font-semibold">Some Things I Believe</h3>
  <ul class="list-disc">
    <li>It&apos;s important to do things FAST!</li>
    <ul class="ml-6 list-[circle]">
      <li>Time is finite resources</li>
      <li>Time is the denominator</li>
      <li>A week is 2% of the year</li>
      <li>Going fast makes you focus on what's important. No wasted time for the unimportant</li>
    </ul>
  </ul>
</div>
