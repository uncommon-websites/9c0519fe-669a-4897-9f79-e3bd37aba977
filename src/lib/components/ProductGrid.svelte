<script lang="ts">
    import ProductCard from './ProductCard.svelte';

    const products = [
        {
            badge: "Bestseller",
            code: "DS-01®",
            title: "Daily Synbiotic",
            image: "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?q=80&w=500&auto=format&fit=crop", 
            price: "$49.99"
        },
        {
            badge: "New",
            code: "DM-02™",
            title: "Daily Multivitamin",
            image: "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?q=80&w=500&auto=format&fit=crop", 
            price: "$39.99"
        },
        {
            badge: "New",
            code: "AM-02™",
            title: "Energy + Focus",
            image: "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?q=80&w=500&auto=format&fit=crop",
            price: "$34.99"
        },
        {
            badge: "New",
            code: "PM-02™",
            title: "Sleep + Restore",
            image: "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?q=80&w=500&auto=format&fit=crop",
            price: "$34.99"
        }
    ];
</script>

<section class="bg-[#1A3026] py-24">
    <div class="container mx-auto px-6 md:px-12">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 text-white">
            <div class="max-w-xl">
                <h2 class="text-4xl md:text-[44px] leading-tight font-medium tracking-tight mb-6">Whole body health starts in the gut.</h2>
                <p class="text-[17px] text-white/80 font-light max-w-md leading-relaxed">Formulations that provide fast-acting and sustained support using scientifically and clinically studied ingredients.</p>
            </div>
            <a href="/" class="hidden md:inline-flex items-center text-[13px] font-bold border-b border-white/30 pb-0.5 hover:border-white transition-colors mt-6 md:mt-0 tracking-wide uppercase">
                Shop All <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
            {#each products as product}
                <ProductCard {...product} isDark={true} />
            {/each}
        </div>

        <div class="mt-12 text-center md:hidden">
            <a href="/" class="inline-flex items-center text-[13px] font-bold border-b border-white/30 pb-0.5 hover:border-white transition-colors text-white tracking-wide uppercase">
                Shop All <span class="ml-2">→</span>
            </a>
        </div>
    </div>
</section>
