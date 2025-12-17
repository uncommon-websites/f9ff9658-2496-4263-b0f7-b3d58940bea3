<script>
  const heroes = [
    {
      name: "EPISODE 1",
      company: "AI Startup Founder",
      image: "/generated/image-ai-startup-founder-in-modern-tech-office-1765988987916-0.webp", 
      alt: "AI startup founder in office"
    },
    {
      name: "EPISODE 2",
      company: "Tech Entrepreneur",
      image: "/generated/image-young-tech-entrepreneur-at-standing-desk-1765988999307-1.webp",
      alt: "Young tech entrepreneur at work"
    },
    {
      name: "EPISODE 3",
      company: "AI Company Founder",
      image: "/generated/image-female-ai-company-founder-in-modern-offi-1765989008746-2.webp",
      alt: "Female AI company founder"
    },
    {
      name: "EPISODE 4",
      company: "Startup Team",
      image: "/generated/image-tech-startup-team-collaborating-in-open--1765989014869-3.webp",
      alt: "Tech startup team collaborating"
    }
  ];
</script>

<section class="pt-32 pb-16 md:pt-48 md:pb-24 overflow-hidden">
  <div class="container mx-auto px-6 md:px-12 mb-16">
    <h1 class="font-display text-5xl md:text-7xl leading-[1.1] text-gray-900 max-w-4xl">
      Capturing <span class="italic font-normal">startup culture</span><br />
      through gonzo journalism.
    </h1>
  </div>

  <div class="pl-6 md:pl-12 overflow-x-auto pb-8 scrollbar-hide">
    <div class="flex space-x-1 min-w-max">
      {#each heroes as hero, i}
        <div class="relative group w-[300px] md:w-[400px]">
          <div class="aspect-[3/4] overflow-hidden bg-gray-100 relative">
            <img 
              src={hero.image} 
              alt={hero.alt}
              class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
            />
            {#if i === 0}
              <button class="absolute bottom-4 left-4 w-8 h-8 bg-white rounded-full flex items-center justify-center hover:scale-110 transition-transform" aria-label="Play">
                <svg width="10" height="12" viewBox="0 0 10 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M1 1L9 6L1 11V1Z" fill="black"/>
                </svg>
              </button>
              <div class="absolute bottom-0 left-0 w-full h-1 bg-gray-200">
                <div class="h-full bg-primary-600 w-1/3"></div>
              </div>
            {/if}
          </div>
          <div class="mt-4 flex items-baseline space-x-2">
            <span class="text-xs font-bold tracking-widest uppercase text-gray-900">{hero.name}</span>
            <span class="text-xs font-serif italic text-gray-500">{hero.company}</span>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
