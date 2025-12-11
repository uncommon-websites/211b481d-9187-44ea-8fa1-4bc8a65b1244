<section class="max-w-[1200px] mx-auto px-4 py-20">
    <div class="grid md:grid-cols-2 gap-12 items-center">
        <!-- Left Content -->
        <div>
            <!-- AI Stamp -->
            <div class="relative w-24 h-24 mb-8">
                <svg width="60" height="60" viewBox="0 0 24 24" fill="none" class="absolute left-0 top-0 transform -rotate-6">
                     <rect x="2" y="2" width="20" height="20" rx="2" stroke="#EF4444" stroke-width="1.5"></rect>
                     <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle" font-family="serif" font-weight="bold" font-size="12" fill="#EF4444">AI</text>
                     <rect x="1" y="1" width="22" height="22" rx="2" stroke="#EF4444" stroke-width="1" stroke-dasharray="2 2"></rect>
                </svg>
                 <svg width="60" height="60" viewBox="0 0 24 24" fill="none" class="absolute left-10 top-0 transform rotate-12">
                     <circle cx="12" cy="12" r="10" stroke="#3B82F6" stroke-width="1.5"></circle>
                     <path d="M8 8L6 12L8 16" stroke="#3B82F6" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                     <path d="M16 8L18 12L16 16" stroke="#3B82F6" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                     <circle cx="12" cy="12" r="11" stroke="#3B82F6" stroke-width="1" stroke-dasharray="2 2"></circle>
                </svg>
            </div>

            <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-notion-black mb-12 text-balance leading-[1.1]">
                Every field extracted, accurately.
            </h2>

            <div class="space-y-8">
                <div class="flex gap-4">
                    <div class="w-6 h-6 flex items-center justify-center text-notion-gray font-mono text-lg">{"{}"}</div>
                    <div>
                        <h3 class="font-semibold text-notion-black text-lg">Custom field extraction</h3>
                        <p class="text-notion-gray mt-1 leading-relaxed">Define any fields you need—invoice numbers, dates, amounts, addresses—and V7 Go extracts them automatically.</p>
                    </div>
                </div>
                 <div class="flex gap-4">
                    <div class="w-6 h-6 flex items-center justify-center text-green-500">
                        <svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"></polyline></svg>
                    </div>
                    <div>
                        <h3 class="font-semibold text-notion-black text-lg">Validation rules</h3>
                        <p class="text-notion-gray mt-1 leading-relaxed">Set business rules to validate extracted data automatically, ensuring accuracy before it enters your systems.</p>
                    </div>
                </div>
                 <div class="flex gap-4">
                    <div class="w-6 h-6 flex items-center justify-center text-blue-500">
                        <svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path></svg>
                    </div>
                    <div>
                        <h3 class="font-semibold text-notion-black text-lg">API integrations</h3>
                        <p class="text-notion-gray mt-1 leading-relaxed">Export structured data directly to your ERP, accounting software, or database via REST API.</p>
                    </div>
                </div>
                 <div class="flex gap-4">
                    <div class="w-6 h-6 flex items-center justify-center text-notion-gray font-serif italic font-bold">AI</div>
                    <div>
                        <h3 class="font-semibold text-notion-black text-lg">Continuous learning</h3>
                        <p class="text-notion-gray mt-1 leading-relaxed">The AI improves with every document, learning your specific formats and requirements.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Visual -->
        <div class="bg-[#F7F7F5] rounded-xl p-8 h-[600px] flex items-center justify-center overflow-hidden">
            <div class="bg-white rounded-lg shadow-xl border border-gray-200 w-full max-w-md p-6 text-sm">
                <div class="flex items-center justify-between mb-4 border-b border-gray-100 pb-4">
                    <div>
                        <div class="font-medium text-notion-black">Invoice_2024_001.pdf</div>
                        <div class="text-xs text-gray-400 mt-1">Processed • 99% confidence</div>
                    </div>
                    <span class="inline-flex items-center px-2 py-1 rounded text-xs font-medium bg-green-100 text-green-700">
                        Verified
                    </span>
                </div>
                
                <!-- Extracted Data -->
                <div class="space-y-4">
                    <div>
                        <div class="text-xs font-medium text-gray-500 mb-1">Vendor Information</div>
                        <div class="bg-gray-50 rounded p-3 space-y-2 text-xs">
                            <div class="flex justify-between">
                                <span class="text-gray-600">Vendor Name:</span>
                                <span class="font-medium text-notion-black">Acme Corporation</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-600">Vendor ID:</span>
                                <span class="font-medium text-notion-black">ACME-2024</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-600">Address:</span>
                                <span class="font-medium text-notion-black">123 Main St, NY</span>
                            </div>
                        </div>
                    </div>

                    <div>
                        <div class="text-xs font-medium text-gray-500 mb-1">Invoice Details</div>
                        <div class="bg-gray-50 rounded p-3 space-y-2 text-xs">
                            <div class="flex justify-between">
                                <span class="text-gray-600">Invoice Number:</span>
                                <span class="font-medium text-notion-black">INV-2024-001</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-600">Date:</span>
                                <span class="font-medium text-notion-black">Jan 15, 2024</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-600">Due Date:</span>
                                <span class="font-medium text-notion-black">Feb 15, 2024</span>
                            </div>
                        </div>
                    </div>

                    <div>
                        <div class="text-xs font-medium text-gray-500 mb-1">Payment Information</div>
                        <div class="bg-blue-50 rounded p-3 space-y-2 text-xs border border-blue-200">
                            <div class="flex justify-between">
                                <span class="text-gray-600">Subtotal:</span>
                                <span class="font-medium text-notion-black">$4,250.00</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-600">Tax (8%):</span>
                                <span class="font-medium text-notion-black">$340.00</span>
                            </div>
                            <div class="flex justify-between border-t border-blue-200 pt-2">
                                <span class="font-semibold text-notion-black">Total Amount:</span>
                                <span class="font-bold text-notion-black">$4,590.00</span>
                            </div>
                        </div>
                    </div>

                    <button class="w-full bg-notion-black text-white text-xs font-medium px-4 py-2 rounded hover:bg-notion-gray transition-colors">
                        Export to Accounting System
                    </button>
                </div>
            </div>
        </div>
    </div>
</section>
