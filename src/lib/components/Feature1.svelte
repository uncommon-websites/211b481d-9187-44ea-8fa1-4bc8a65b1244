<section class="max-w-[1000px] mx-auto px-4 py-20">
    <div class="flex flex-col md:flex-row justify-between items-start mb-12">
        <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-notion-black max-w-lg text-balance leading-[1.1]">
            Every document classified, automatically.
        </h2>
        <!-- Stamps Illustration -->
        <div class="mt-8 md:mt-0 relative">
             <!-- Bell Stamp -->
            <svg width="60" height="60" viewBox="0 0 24 24" fill="none" stroke="#F59E0B" stroke-width="1.5" class="absolute -left-12 top-0 transform -rotate-12">
                <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
                <path d="M13.73 21a2 2 0 0 1-3.46 0"></path>
                <rect x="1" y="1" width="22" height="22" rx="2" stroke-dasharray="2 2"></rect>
            </svg>
            <!-- Envelope Stamp -->
             <svg width="60" height="60" viewBox="0 0 24 24" fill="none" stroke="#EF4444" stroke-width="1.5" class="absolute left-4 top-4 transform rotate-6 z-10 bg-white">
                <rect x="2" y="4" width="20" height="16" rx="2"></rect>
                <path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path>
                 <rect x="1" y="1" width="22" height="22" rx="2" stroke-dasharray="2 2"></rect>
            </svg>
             <!-- Blue Stamp -->
             <svg width="60" height="60" viewBox="0 0 24 24" fill="none" stroke="#3B82F6" stroke-width="1.5" class="absolute left-20 -top-2 transform -rotate-6">
                <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"></path>
                 <rect x="1" y="1" width="22" height="22" rx="2" stroke-dasharray="2 2"></rect>
            </svg>
        </div>
    </div>

    <div class="bg-[#F7F7F5] rounded-xl p-8 md:p-12 overflow-hidden relative min-h-[500px]">
        <!-- Background UI -->
        <div class="bg-white rounded-lg shadow-sm border border-gray-200 max-w-3xl mx-auto p-6 opacity-50 blur-[1px]">
            <div class="flex items-center justify-between mb-6">
                <div class="flex items-center gap-2 font-medium text-notion-black">
                    <svg class="w-5 h-5 text-red-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect><line x1="16" y1="2" x2="16" y2="6"></line><line x1="8" y1="2" x2="8" y2="6"></line><line x1="3" y1="10" x2="21" y2="10"></line></svg>
                    Inbox
                </div>
                <div class="flex items-center gap-2 border border-gray-200 rounded px-2 py-1 text-sm">
                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                    Auto label
                </div>
            </div>
            <div class="space-y-4">
                {#each [1, 2, 3, 4, 5] as i}
                    <div class="flex items-center gap-4">
                        <div class="w-24 h-3 bg-gray-100 rounded"></div>
                        <div class="flex-1 h-3 bg-gray-100 rounded"></div>
                    </div>
                {/each}
            </div>
        </div>

        <!-- Foreground Popover -->
        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full max-w-md bg-white rounded-xl shadow-2xl border border-gray-200 p-2 z-10">
            <div class="px-3 py-2 text-xs font-medium text-gray-500">Suggested</div>
            <div class="space-y-1">
                <div class="flex items-start gap-3 p-2 hover:bg-gray-50 rounded cursor-pointer">
                    <svg class="w-4 h-4 text-gray-400 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline></svg>
                    <span class="text-sm text-notion-black">Invoices with payment terms</span>
                </div>
                <div class="flex items-start gap-3 p-2 hover:bg-gray-50 rounded cursor-pointer">
                    <svg class="w-4 h-4 text-gray-400 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path></svg>
                    <span class="text-sm text-notion-black">Contracts requiring review</span>
                </div>
                <div class="flex items-start gap-3 p-2 hover:bg-gray-50 rounded cursor-pointer">
                    <svg class="w-4 h-4 text-gray-400 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect></svg>
                    <span class="text-sm text-notion-black">Receipts for expense reports</span>
                </div>
            </div>
        </div>
    </div>

    <p class="mt-8 text-lg text-notion-black max-w-2xl">
        Train V7 Go on your document types, and it'll automatically classify and extract data as documents arrive—no manual sorting required.
    </p>
</section>
