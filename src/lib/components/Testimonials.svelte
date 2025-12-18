<script lang="ts">
</script>

<section class="bg-white py-24">
    <div class="container mx-auto px-6 md:px-12 text-center">
        <h2 class="text-4xl md:text-[44px] leading-tight font-medium tracking-tight mb-4 text-[#191919]">
            Over 1 million health<br/>
            transformations (and counting).
        </h2>
        <p class="text-[13px] text-[#191919]/60 font-medium mb-16 tracking-wide">
            See how real people are changing their health with Seed.
        </p>

        <!-- Video Carousel Placeholder -->
        <div class="flex gap-6 overflow-x-auto pb-8 snap-x no-scrollbar items-center justify-center">
            <!-- Card 1 (Large) -->
            <div class="min-w-[80vw] md:min-w-[800px] aspect-video bg-[#F4F4F0] rounded-lg relative overflow-hidden group snap-center cursor-pointer shadow-xl">
                <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=1000&auto=format&fit=crop" alt="Testimonial" class="w-full h-full object-cover" />
                <div class="absolute inset-0 bg-black/10 group-hover:bg-black/5 transition-colors"></div>
                <div class="absolute bottom-8 left-8 text-white text-left">
                    <h3 class="text-xl font-medium tracking-tight opacity-90">Seed®</h3>
                </div>
                <div class="absolute bottom-8 right-8 text-white text-right">
                    <h3 class="text-xl font-medium tracking-tight">DS-01® Member Experiences</h3>
                </div>
                <div class="absolute top-6 right-6 text-white bg-black/20 p-2 rounded-full backdrop-blur-sm hover:bg-black/30 transition-colors">
                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <path d="M15 3h6v6M9 21H3v-6M21 3l-7 7M3 21l7-7" />
                    </svg>
                </div>
            </div>
             <!-- Card 2 (Peek) -->
             <div class="min-w-[300px] md:min-w-[400px] aspect-[9/16] md:aspect-video bg-[#F4F4F0] rounded-lg relative overflow-hidden group snap-center opacity-50 hidden md:block">
                <img src="https://images.unsplash.com/photo-1517841905240-472988babdf9?q=80&w=1000&auto=format&fit=crop" alt="Testimonial" class="w-full h-full object-cover grayscale" />
                 <div class="absolute inset-0 bg-black/20"></div>
                 <div class="absolute bottom-8 left-8 text-white text-left">
                    <h3 class="text-xl font-medium tracking-tight">Seed®</h3>
                </div>
            </div>
        </div>

        <!-- Controls -->
        <div class="flex items-center justify-center gap-4 mt-8">
            <button class="w-10 h-10 rounded-full bg-[#1A3026] text-white flex items-center justify-center hover:bg-[#243E32] transition-colors" aria-label="Pause video">
                <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor">
                    <rect x="6" y="4" width="4" height="16" />
                    <rect x="14" y="4" width="4" height="16" />
                </svg>
            </button>
            <div class="flex items-center gap-3 text-[11px] font-bold uppercase tracking-widest bg-[#F4F4F0] pl-4 pr-1 py-1 rounded-full">
                <span>▶ Zam</span>
                <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=100&auto=format&fit=crop" class="w-8 h-8 rounded-full object-cover" alt="Zam" />
            </div>
        </div>
    </div>
</section>
