<script lang="ts">
	// Navbar component
</script>

<nav class="flex items-center justify-between px-4 py-3 bg-white sticky top-0 z-50 border-b border-transparent transition-all duration-200">
	<div class="flex items-center gap-6">
		<a href="/" class="flex items-center gap-2">
			<span class="font-bold text-2xl tracking-tight text-notion-black">V7 Go</span>
		</a>

		<div class="hidden lg:flex items-center gap-5 text-[14px] font-normal text-notion-gray">
			<a href="#" class="hover:text-notion-black transition-colors">Platform</a>
			<a href="#" class="hover:text-notion-black transition-colors">Solutions</a>
			<a href="#" class="hover:text-notion-black transition-colors">Enterprise</a>
			<a href="#" class="hover:text-notion-black transition-colors">Pricing</a>
			<div class="group relative flex items-center gap-1 cursor-pointer hover:text-notion-black transition-colors">
				Resources
				<svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
				</svg>
			</div>
			<a href="#" class="hover:text-notion-black transition-colors">Request a demo</a>
		</div>
	</div>

	<div class="flex items-center gap-4">
		<a href="#" class="text-[14px] font-normal text-notion-gray hover:text-notion-black transition-colors hidden sm:block">Log in</a>
		<a href="#" class="bg-notion-black text-white text-[14px] font-medium px-3 py-1.5 rounded-[4px] hover:bg-notion-gray transition-colors">Start free trial</a>
	</div>
</nav>
