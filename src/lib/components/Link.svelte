<script>
	export let name = 'Link';
	export let href = 'https://hisamafahri';
	export let display = '@hisamafahri';
	export let target = undefined;
</script>

<div class="flex flex-row items-start justify-start text-sm mt-4">
	<p class="text-gray-500 mr-4 w-32">{name}</p>
	<a class="flex flex-row items-center justify-start text-gray-700 hover:underline" {href} {target}
		>{display}
		{#if target}
			<svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 20 20"
				fill="currentColor"
				class="w-4 h-4"
			>
				<path
					fill-rule="evenodd"
					d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z"
					clip-rule="evenodd"
				/>
			</svg>
		{/if}
	</a>
</div>
