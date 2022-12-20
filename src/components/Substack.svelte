<script>
	let isNewsletterOpen = true;
	function toggleNewsletter() {
		isNewsletterOpen = !isNewsletterOpen;
	}
	function onSubmit() {
		alert(
			'This newsletter section is not yet implemented! if you are seeing this outside of swyxkit then go remind the site author to update Newsletter.svelte.'
		);
	}
</script>

<section class="mb-16 w-full" id="newsletter">
	<div
		class="my-4 w-full border-y border-gray-300 bg-gray-50 p-6 dark:border-gray-600 dark:bg-gray-900 sm:rounded sm:border-x items"
	>
		<div class="flex items-center pb-4 justify-between space-x-4 text-gray-900 dark:text-gray-100">
			<p class="text-lg font-bold md:text-xl">Subscribe to the newsletter</p>

			<button
				aria-label="Toggle Newsletter CTA"
				class="flex h-9 w-9  items-center justify-center rounded-lg ring-gray-300 transition-all hover:ring-2"
				on:click={toggleNewsletter}
			>
				{#if isNewsletterOpen}
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="h-5 w-5"
						viewBox="0 0 20 20"
						fill="currentColor"
					>
						<path
							fill-rule="evenodd"
							d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
							clip-rule="evenodd"
						/>
					</svg>
				{:else}
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="h-5 w-5"
						viewBox="0 0 20 20"
						fill="currentColor"
					>
						<path
							fill-rule="evenodd"
							d="M15.707 4.293a1 1 0 010 1.414l-5 5a1 1 0 01-1.414 0l-5-5a1 1 0 011.414-1.414L10 8.586l4.293-4.293a1 1 0 011.414 0zm0 6a1 1 0 010 1.414l-5 5a1 1 0 01-1.414 0l-5-5a1 1 0 111.414-1.414L10 14.586l4.293-4.293a1 1 0 011.414 0z"
							clip-rule="evenodd"
						/>
					</svg>
				{/if}
			</button>
		</div>
    <div class="flex justify-center">
      {#if isNewsletterOpen}
        <iframe src="https://successfuldesi.substack.com/embed" width="480" height="320" style="border:1px solid #EEE; background:; #EFF6FF" frameborder="0" scrolling="no" title="substack"></iframe>
      {/if}
    </div>
	</div>
</section>
