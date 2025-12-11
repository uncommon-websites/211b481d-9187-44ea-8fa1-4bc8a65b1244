<script lang="ts">
	const links = {
		Company: ["About us", "Careers", "Security", "Status", "Terms & privacy", "Your privacy rights"],
		Product: ["API Documentation", "Integrations", "Pricing", "Use Cases"],
		Resources: ["Help center", "Blog", "Case studies", "Documentation", "Partner programs"],
		"Solutions": ["Finance & Accounting", "Healthcare", "Legal", "Logistics"]
	};
</script>

<footer class="border-t border-notion-border py-16 px-4 md:px-8 lg:px-16 bg-white text-[14px]">
	<div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-6 gap-8">
		<div class="lg:col-span-2 flex flex-col gap-6">
			<div class="flex items-center gap-2">
				<span class="font-bold text-2xl tracking-tight text-notion-black">V7 Go</span>
			</div>
			
			<div class="flex gap-4 text-notion-gray">
				<!-- Social Icons -->
				<a href="#" aria-label="Instagram"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg></a>
				<a href="#" aria-label="Twitter"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"></path></svg></a>
				<a href="#" aria-label="LinkedIn"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg></a>
				<a href="#" aria-label="Facebook"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path></svg></a>
				<a href="#" aria-label="YouTube"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.33 29 29 0 0 0-.46-5.33z"></path><polygon points="9.75 15.02 15.5 11.75 9.75 8.48 9.75 15.02"></polygon></svg></a>
			</div>

			<div class="mt-4">
				<button class="flex items-center gap-2 bg-gray-100 hover:bg-gray-200 px-3 py-2 rounded text-notion-gray transition-colors">
					<svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><line x1="2" y1="12" x2="22" y2="12"></line><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path></svg>
					English (US)
					<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="6 9 12 15 18 9"></polyline></svg>
				</button>
			</div>

            <div class="mt-auto pt-8 text-gray-500 text-xs">
                <p>Do Not Sell or Share My Info</p>
                <p class="mt-1">Cookie settings</p>
                <p class="mt-4">© 2025 V7 Go, Inc.</p>
            </div>
		</div>

		{#each Object.entries(links) as [category, items]}
			<div class="flex flex-col gap-3">
				<h3 class="font-semibold text-notion-black mb-1">{category}</h3>
				{#each items as item}
					<a href="#" class="text-notion-gray hover:text-notion-blue hover:underline transition-colors">{item}</a>
				{/each}
                {#if category === "Solutions"}
                    <a href="#" class="font-medium text-notion-black flex items-center gap-1 mt-4 hover:text-notion-blue hover:underline transition-colors">
                        View all solutions
                        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg>
                    </a>
                {/if}
			</div>
		{/each}
	</div>
</footer>
