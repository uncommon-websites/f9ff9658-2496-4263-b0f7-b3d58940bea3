<script>
  import Header from '$lib/components/Header.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import Philosophy from '$lib/components/Philosophy.svelte';
  import Featured from '$lib/components/Featured.svelte';
  import NewsGrid from '$lib/components/NewsGrid.svelte';
  import Industries from '$lib/components/Industries.svelte';
  import Testimonial from '$lib/components/Testimonial.svelte';
  import PinkSection from '$lib/components/PinkSection.svelte';
  import BlackSection from '$lib/components/BlackSection.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<div class="bg-white min-h-screen font-body selection:bg-primary-600 selection:text-white">
  <Header />
  
  <main>
    <Hero />
    <Philosophy />
    <Featured />
    <NewsGrid />
    <Industries />
    <Testimonial />
    <PinkSection />
    <BlackSection />
  </main>

  <Footer />
  
  <!-- Floating Accessibility/Location Icon (bottom left in screenshot) -->
  <div class="fixed bottom-6 left-6 z-40 hidden md:block">
    <button class="w-8 h-8 rounded-full border border-gray-300 flex items-center justify-center text-gray-500 hover:border-black hover:text-black transition-colors bg-white">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
        <circle cx="12" cy="12" r="10"></circle>
        <path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path>
        <path d="M2 12h20"></path>
      </svg>
    </button>
  </div>
</div>

