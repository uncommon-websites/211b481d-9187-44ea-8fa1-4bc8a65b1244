<script>
    // Testimonials Component
    const testimonials = [
        {
            name: "Sarah Chen",
            handle: "CFO, TechCorp",
            text: "V7 Go reduced our invoice processing time from days to minutes. The accuracy is incredible—we've eliminated manual data entry errors completely."
        },
        {
            name: "Marcus Rodriguez",
            handle: "Operations Director",
            text: "The AI understands complex document structures that other tools miss. It's like having a team of data entry specialists working 24/7."
        },
        {
            name: "Emily Watson",
            handle: "Finance Manager",
            text: "V7 Go handles everything from receipts to contracts seamlessly. The confidence scores give us peace of mind about data quality."
        },
        {
            name: "David Park",
            handle: "Head of Procurement",
            text: "We process thousands of purchase orders monthly. V7 Go's automation has been transformative for our team's productivity."
        }
    ];
</script>

<section class="py-16 overflow-hidden">
    <div class="flex gap-6 overflow-x-auto px-4 pb-8 md:justify-center no-scrollbar snap-x">
        {#each testimonials as t}
            <div class="flex-none w-[300px] md:w-[350px] p-6 bg-white border border-gray-100 rounded-xl shadow-sm snap-center">
                <div class="flex flex-col gap-4 h-full">
                    <div>
                        <div class="font-medium text-notion-black">{t.name}</div>
                        <div class="text-gray-400 text-sm">{t.handle}</div>
                    </div>
                    <p class="text-notion-gray text-[15px] leading-relaxed">
                        {t.text}
                    </p>
                </div>
            </div>
        {/each}
        <!-- Add a fade effect or just let it scroll. The screenshot shows them cut off on the right, implying scroll or just a grid. -->
    </div>
</section>

<style>
    .no-scrollbar::-webkit-scrollbar {
        display: none;
    }
    .no-scrollbar {
        -ms-overflow-style: none;
        scrollbar-width: none;
    }
</style>
