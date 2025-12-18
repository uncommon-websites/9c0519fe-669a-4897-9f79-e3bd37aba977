<script lang="ts">
</script>

<section class="relative h-screen min-h-[700px] w-full overflow-hidden bg-[#8C8C84]">
    <!-- Background Image -->
    <div class="absolute inset-0 w-full h-full">
        <img 
            src="https://images.unsplash.com/photo-1616394584738-fc6e612e71b9?q=80&w=2940&auto=format&fit=crop" 
            alt="Hand reaching for bowl" 
            class="w-full h-full object-cover"
        />
        <div class="absolute inset-0 bg-black/10"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 h-full container mx-auto px-6 md:px-12 flex flex-col justify-center text-white pb-10 pt-20">
        <div class="max-w-2xl">
            <!-- Badge -->
            <span class="inline-block bg-[#D4E995] text-[#191919] text-[10px] font-bold px-2 py-0.5 rounded mb-6 tracking-wide uppercase">
                New
            </span>

            <!-- Heading -->
            <h1 class="text-[42px] md:text-[56px] lg:text-[64px] leading-[1.05] font-normal tracking-tight mb-6">
                Nutrition, energy, and sleep—<br class="hidden md:block" />
                advanced by microbiome science
            </h1>

            <!-- Subtext -->
            <p class="text-base md:text-lg text-white/90 mb-10 max-w-lg leading-relaxed font-light">
                Seed's Co-Biotics nourish you and your microbiome to deliver targeted, daily benefits.
            </p>

            <!-- CTA -->
            <div class="flex items-center gap-4">
                <a href="/" class="inline-block bg-white text-[#191919] px-8 py-3.5 rounded-full font-medium text-[13px] hover:bg-gray-100 transition-colors tracking-wide">
                    Shop Now
                </a>
                <div class="text-[10px] uppercase tracking-widest text-white/80 border-l border-white/30 pl-4 ml-2 leading-tight">
                    Dietary Supplement<br/>
                    30 Capsules — 30 Day Supply
                </div>
            </div>
        </div>
    </div>

    <!-- Pause Button (Bottom Right) -->
    <div class="absolute bottom-8 right-8 z-20">
        <button class="w-8 h-8 rounded-full border border-white/40 flex items-center justify-center text-white hover:bg-white/10 transition-colors backdrop-blur-sm" aria-label="Pause video">
            <svg width="10" height="10" viewBox="0 0 10 10" fill="currentColor">
                <rect x="2" y="2" width="2" height="6" />
                <rect x="6" y="2" width="2" height="6" />
            </svg>
        </button>
    </div>
</section>
