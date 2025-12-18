<script lang="ts">
    export let badge = "";
    export let title = "";
    export let code = "";
    export let image = "";
    export let price = "";
    export let link = "/";
    export let isDark = false;
</script>

<div class="group relative flex flex-col items-center text-center p-8 rounded-lg bg-[#243E32] transition-all duration-300 hover:transform hover:-translate-y-1 h-full">
    {#if badge}
        <div class="absolute top-6 left-6 bg-[#D4E995] text-[#191919] text-[10px] font-bold px-2 py-0.5 rounded-sm uppercase tracking-wide">
            {badge}
        </div>
    {/if}

    <div class="mt-8 mb-6 w-14 h-14 rounded-full border border-white/20 flex items-center justify-center text-white text-[10px] tracking-widest font-medium">
        {code}
    </div>

    <h3 class="text-white text-xl font-medium mb-8 leading-tight px-4">{title}</h3>

    <div class="relative w-full flex-grow flex items-center justify-center mb-10">
        <!-- Image -->
        <img src={image} alt={title} class="w-40 h-auto object-contain drop-shadow-2xl group-hover:scale-105 transition-transform duration-500" />
    </div>

    <div class="mt-auto w-full flex flex-col items-center">
        <a href={link} class="block w-full max-w-[180px] py-3.5 rounded-full text-[11px] font-bold uppercase tracking-widest transition-colors mb-3 bg-[#13241C] text-white hover:bg-[#1a3026]">
            Shop Now
        </a>
        <p class="text-white/60 text-[10px] tracking-wide">Starting at {price} per month</p>
    </div>
</div>
