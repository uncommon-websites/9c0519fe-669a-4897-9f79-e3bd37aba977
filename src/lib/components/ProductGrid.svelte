<script lang="ts">
    import ProductCard from './ProductCard.svelte';

    const products = [
        {
            badge: "Popular",
            code: "WINE",
            title: "Curated Wines",
            image: "/generated/image-premium-red-wine-bottle-on-a-minimalist--1766918509791-1.webp", 
            price: "$24"
        },
        {
            badge: "Trending",
            code: "SPIRITS",
            title: "Premium Spirits",
            image: "/generated/image-craft-whisky-bottle-with-amber-liquid-in-1766918511928-2.webp", 
            price: "$45"
        },
        {
            badge: "New",
            code: "BEER",
            title: "Craft Beer",
            image: "/generated/image-craft-beer-bottles-in-ice-bucket-at-casu-1766918514208-3.webp",
            price: "$18"
        },
        {
            badge: "Curated",
            code: "SETS",
            title: "Tasting Sets",
            image: "/generated/image-curated-selection-of-wine-bottles-arrang-1766918516545-4.webp",
            price: "$89"
        }
    ];
</script>

<section class="bg-[#191919] py-24">
    <div class="container mx-auto px-6 md:px-12">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 text-white">
            <div class="max-w-xl">
                <h2 class="text-4xl md:text-[44px] leading-tight font-medium tracking-tight mb-6">Confidence in choice, delivered.</h2>
                <p class="text-[17px] text-white/80 font-light max-w-md leading-relaxed">A tightly curated range of wine, spirits, and beer—selected to match your taste and backed by clear, explainable recommendations.</p>
            </div>
            <a href="/" class="hidden md:inline-flex items-center text-[13px] font-bold border-b border-white/30 pb-0.5 hover:border-white transition-colors mt-6 md:mt-0 tracking-wide uppercase">
                Explore All <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
            {#each products as product}
                <ProductCard {...product} isDark={true} />
            {/each}
        </div>

        <div class="mt-12 text-center md:hidden">
            <a href="/" class="inline-flex items-center text-[13px] font-bold border-b border-white/30 pb-0.5 hover:border-white transition-colors text-white tracking-wide uppercase">
                Explore All <span class="ml-2">→</span>
            </a>
        </div>
    </div>
</section>
