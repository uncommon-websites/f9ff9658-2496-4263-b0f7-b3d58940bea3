<section class="py-24 md:py-32">
  <div class="container mx-auto px-6 md:px-12 text-center">
    <p class="text-gray-500 text-lg mb-12 font-light">Featured AI companies we've covered:</p>
    
    <div class="max-w-3xl mx-auto">
      {#each ['Anthropic', 'Perplexity', 'Mistral AI', 'Cohere'] as company}
        <div class="border-t border-gray-200 py-6 md:py-8 group cursor-pointer hover:bg-gray-50 transition-colors">
          <h3 class="font-display text-4xl md:text-5xl text-gray-500 group-hover:text-black transition-colors">
            {company}
          </h3>
        </div>
      {/each}
      <div class="border-t border-gray-200"></div>
    </div>

    <div class="mt-16">
      <a href="/companies" class="inline-flex items-center px-8 py-3 border border-gray-300 rounded-full text-sm font-medium text-gray-500 hover:text-black hover:border-black transition-colors">
        See all episodes
      </a>
    </div>
  </div>
</section>
