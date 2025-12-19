<script>
  import Header from '$lib/components/Header.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import Logos from '$lib/components/Logos.svelte';
  import ValueProp from '$lib/components/ValueProp.svelte';
  import Products from '$lib/components/Products.svelte';
  import Features from '$lib/components/Features.svelte';
  import Testimonial from '$lib/components/Testimonial.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
  <title>Tipple - Unified Alcohol Commerce Infrastructure</title>
  <meta name="description" content="Integrated compliance, logistics, and payment systems that power the $1.6T alcohol market. Pre-built ERP connectors for distributors and brands." />
</svelte:head>

<Header />

<main class="bg-white overflow-hidden">
  <Hero />
  <Logos />
  <ValueProp />
  <Products />
  <Features />
  <Testimonial />
</main>

<Footer />

