<script>
	export let title = 'Untitled project';
	export let href = '#';
	export let description = 'No description available';
</script>

<a
	class="w-full transform rounded-xl bg-gradient-to-r from-yellow-400 via-red-500 to-pink-500 p-1 transition-all hover:scale-[1.01] md:w-1/3 group"
	{href}
	target="_blank"
	rel="noopener noreferrer"
	><div class="flex h-full flex-col justify-between rounded-lg bg-white p-4 dark:bg-gray-900 relative overflow-hidden">
		<div class="flex flex-col justify-between md:flex-row">
			<h4
				class="mb-6 w-full text-lg font-medium tracking-tight text-gray-900 dark:text-gray-100 sm:mb-10 md:text-lg"
			>
				{title}
			</h4>
		</div>
		
		<!-- Hover description overlay -->
		<div class="absolute inset-0 bg-gray-900 bg-opacity-90 text-white p-4 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 rounded-lg">
			<p class="text-sm text-center leading-relaxed">
				{description}
			</p>
		</div>
		
		<div class="capsize flex items-center text-gray-800 dark:text-gray-200">
			<span class="text-sm font-medium">View Project →</span>
		</div>
	</div></a
>
