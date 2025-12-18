<script lang="ts">
	import Navbar from "$lib/components/Navbar.svelte";
	import Hero from "$lib/components/Hero.svelte";
	import ProductGrid from "$lib/components/ProductGrid.svelte";
	import BundleSection from "$lib/components/BundleSection.svelte";
	import ScienceSection from "$lib/components/ScienceSection.svelte";
	import InfoSection from "$lib/components/InfoSection.svelte";
	import Testimonials from "$lib/components/Testimonials.svelte";
	import Stories from "$lib/components/Stories.svelte";
	import DualPromo from "$lib/components/DualPromo.svelte";
	import Footer from "$lib/components/Footer.svelte";
</script>

<main class="w-full min-h-screen bg-white">
	<Navbar />
	<Hero />
	<ProductGrid />
	<BundleSection />
	<ScienceSection />
	<InfoSection />
	<Testimonials />
	<Stories />
	<DualPromo />
	<Footer />
</main>

