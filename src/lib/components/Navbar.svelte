<script lang="ts">
  import { onMount } from 'svelte';

  let isScrolled = false;

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 50;
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  });
</script>

<div class="fixed w-full z-50 transition-colors duration-300 top-0 left-0 text-seed-black font-sans">
  <!-- Top Bar -->
  <div class="bg-[#f2f2ed] text-[11px] font-medium tracking-wide text-center py-2.5 flex justify-center items-center gap-1 cursor-pointer hover:underline">
    <span>Is DS-01® Daily Synbiotic Right For You?</span>
    <span class="text-[10px]">➜</span>
  </div>

  <!-- Main Nav -->
  <nav class="flex justify-between items-center px-6 py-4 md:px-10 transition-all duration-300 {isScrolled ? 'bg-white/90 backdrop-blur-md shadow-sm py-3 text-seed-black' : 'bg-transparent text-white'}">
    <!-- Left Links -->
    <div class="hidden md:flex items-center gap-8 text-[13px] font-medium tracking-wide">
      <a href="/" class="hover:opacity-60 transition-opacity">Shop</a>
      <a href="/" class="hover:opacity-60 transition-opacity">Science</a>
      <a href="/" class="hover:opacity-60 transition-opacity">Learn</a>
    </div>

    <!-- Logo -->
    <div class="absolute left-1/2 transform -translate-x-1/2">
      <a href="/" class="block flex items-center gap-1">
        <span class="text-2xl font-bold tracking-tight">Seed</span>
        <div class="w-2 h-2 rounded-full bg-current mt-1"></div>
      </a>
    </div>

    <!-- Right Links -->
    <div class="flex items-center gap-6 md:gap-8">
      <a href="/" class="text-[13px] font-medium tracking-wide hover:opacity-60 transition-opacity hidden md:block">Login</a>
      <a href="/" class="{isScrolled ? 'bg-seed-black text-white' : 'bg-white text-seed-black'} px-5 py-2 rounded-full text-[13px] font-bold tracking-wide hover:opacity-90 transition-all shadow-sm">Get Started</a>
      <button class="md:hidden">
        <!-- Mobile Menu Icon -->
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
        </svg>
      </button>
    </div>
  </nav>
</div>

<style>
    /* Adjust logo to match screenshot circle */
    /* The screenshot shows "Seed" text next to a circle or just a circle? 
       Actually looking closer at the screenshot, the logo is "Seed" text with a circle dot maybe? 
       Or just "Seed". Let's look at the screenshot again.
       Top left of nav: "Shop Science Learn".
       Center: "Seed" text logo.
       Right: "Login Get Started".
    */
</style>
