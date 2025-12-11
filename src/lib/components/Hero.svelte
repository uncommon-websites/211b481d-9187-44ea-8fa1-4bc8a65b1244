<script>
    // Hero Component
    const documents = [
        { name: "Invoice_2024_001.pdf", type: "Invoice", status: "Processed", confidence: "99%" },
        { name: "Contract_Vendor_A.pdf", type: "Contract", status: "Processing", confidence: "—" },
        { name: "Receipt_Office.jpg", type: "Receipt", status: "Processed", confidence: "97%" },
        { name: "Form_W9_Supplier.pdf", type: "Tax Form", status: "Processed", confidence: "98%" },
        { name: "PO_12345.pdf", type: "Purchase Order", status: "Processed", confidence: "99%" },
    ];
</script>

<section class="pt-20 pb-16 px-4 flex flex-col items-center text-center max-w-[1200px] mx-auto">
    <!-- Document Icon -->
    <div class="mb-8 relative">
        <svg width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" class="text-notion-black w-20 h-20">
            <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path>
            <polyline points="14 2 14 8 20 8"></polyline>
            <line x1="16" y1="13" x2="8" y2="13"></line>
            <line x1="16" y1="17" x2="8" y2="17"></line>
            <polyline points="10 9 9 9 8 9"></polyline>
        </svg>
        <!-- Sparkle effect -->
        <div class="absolute -right-2 -top-2 w-4 h-4 text-primary-500">
            <svg viewBox="0 0 24 24" fill="currentColor">
                <path d="M12 2L14 10L22 12L14 14L12 22L10 14L2 12L10 10L12 2Z"/>
            </svg>
        </div>
    </div>

    <h1 class="text-5xl md:text-6xl lg:text-7xl font-bold tracking-tight text-notion-black mb-6 max-w-4xl text-balance leading-[1.1]">
        Turn documents into <br class="hidden md:block" /> structured data instantly
    </h1>

    <p class="text-xl text-notion-gray max-w-2xl mb-10 text-balance leading-relaxed">
        V7 Go uses AI to extract, classify, and process any document—from invoices to contracts—with human-level accuracy.
    </p>

    <button class="bg-notion-black text-white text-lg font-medium px-6 py-3 rounded-[6px] hover:bg-notion-gray transition-colors mb-20">
        Start free trial
    </button>

    <!-- UI Mockup - Document Processing Interface -->
    <div class="w-full bg-white rounded-xl shadow-2xl border border-gray-200 overflow-hidden text-left text-sm h-[600px] relative">
        <div class="flex h-full">
            <!-- Sidebar -->
            <div class="w-64 bg-[#F7F7F5] border-r border-gray-200 p-4 flex flex-col gap-6 hidden md:flex">
                <div>
                    <div class="flex items-center gap-2 px-2 py-1 mb-4">
                        <span class="font-bold text-lg text-notion-black">V7 Go</span>
                    </div>
                    
                    <div class="relative mb-4">
                        <svg class="absolute left-2 top-1.5 w-4 h-4 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
                        <input type="text" placeholder="Search documents" class="w-full bg-white border border-gray-200 rounded pl-8 pr-2 py-1 text-sm outline-none placeholder-gray-400">
                    </div>
                </div>

                <div>
                    <div class="text-xs font-medium text-gray-500 px-2 mb-2">Document Types</div>
                    <div class="space-y-0.5">
                        <div class="flex items-center gap-2 px-2 py-1.5 bg-white rounded shadow-sm text-notion-black font-medium">
                            <svg class="w-4 h-4 text-blue-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline></svg>
                            All Documents
                        </div>
                        <div class="flex items-center gap-2 px-2 py-1.5 text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
                            <svg class="w-4 h-4 text-green-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="8" y1="12" x2="16" y2="12"></line><line x1="12" y1="8" x2="12" y2="16"></line></svg>
                            Invoices
                        </div>
                        <div class="flex items-center gap-2 px-2 py-1.5 text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
                            <svg class="w-4 h-4 text-purple-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path></svg>
                            Contracts
                        </div>
                        <div class="flex items-center gap-2 px-2 py-1.5 text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
                            <svg class="w-4 h-4 text-orange-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"></path></svg>
                            Receipts
                        </div>
                        <div class="flex items-center gap-2 px-2 py-1.5 text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
                            <svg class="w-4 h-4 text-red-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path></svg>
                            Tax Forms
                        </div>
                    </div>
                </div>
            </div>

            <!-- Main Content -->
            <div class="flex-1 flex flex-col min-w-0 bg-white">
                <div class="h-12 border-b border-gray-100 flex items-center px-6 justify-between">
                    <div class="flex items-center gap-2 font-medium text-notion-black">
                        <svg class="w-4 h-4 text-blue-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline></svg>
                        All Documents
                    </div>
                    <div class="flex items-center gap-3 text-gray-400">
                        <div class="flex items-center gap-1 text-xs font-medium border border-gray-200 rounded px-2 py-1 text-gray-600">
                            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path></svg>
                            AI Processing
                        </div>
                    </div>
                </div>

                <div class="flex-1 overflow-auto">
                    <table class="w-full text-left border-collapse">
                        <thead class="text-gray-400 text-xs font-normal border-b border-gray-100">
                            <tr>
                                <th class="py-2 pl-6 pr-4 font-normal w-[35%]">Document Name</th>
                                <th class="py-2 px-4 font-normal w-[20%]">Type</th>
                                <th class="py-2 px-4 font-normal w-[20%]">Status</th>
                                <th class="py-2 px-4 font-normal w-[25%]">Confidence</th>
                            </tr>
                        </thead>
                        <tbody class="text-sm">
                            {#each documents as doc}
                                <tr class="group hover:bg-gray-50 border-b border-gray-50 last:border-0 transition-colors">
                                    <td class="py-3 pl-6 pr-4 text-notion-black font-medium truncate flex items-center gap-2">
                                        <svg class="w-4 h-4 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline></svg>
                                        {doc.name}
                                    </td>
                                    <td class="py-3 px-4 text-gray-600 truncate">{doc.type}</td>
                                    <td class="py-3 px-4">
                                        <span class="inline-flex items-center px-2 py-0.5 rounded text-xs font-medium {doc.status === 'Processed' ? 'bg-green-100 text-green-700' : 'bg-blue-100 text-blue-700'}">
                                            {doc.status}
                                        </span>
                                    </td>
                                    <td class="py-3 px-4 text-gray-600">{doc.confidence}</td>
                                </tr>
                            {/each}
                        </tbody>
                    </table>
                </div>
                
                <!-- Floating Action Button -->
                <div class="absolute bottom-8 right-8 bg-primary-600 hover:bg-primary-700 text-white px-4 py-2 rounded-full shadow-lg flex items-center gap-2 cursor-pointer transition-all z-10">
                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"></line><line x1="5" y1="12" x2="19" y2="12"></line></svg>
                    Upload Documents
                </div>
            </div>
        </div>
    </div>
</section>
