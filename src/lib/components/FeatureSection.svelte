<script lang="ts">
  export let align: 'left' | 'right' = 'right';
  export let category: string = '';
  export let title: string = '';
  export let description: string = '';
  export let ctaText: string = '';
  
  interface Testimonial {
    quote: string;
    author: string;
    role: string;
    avatar?: string;
    readStory?: boolean;
  }

  export let testimonial: Testimonial | null = null;
  
  interface Stat {
    value: string;
    label: string;
  }

  export let stats: Stat[] = [];
  export let colorClass: string = 'bg-yellow-400';
</script>

<section class="py-20 bg-white overflow-hidden">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex flex-col lg:flex-row gap-16 items-center">
      
      <!-- Text Content -->
      <div class="flex-1 {align === 'left' ? 'lg:order-2' : 'lg:order-1'}">
        <div class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-4">{category}</div>
        <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 mb-6 leading-tight">
          {title}
        </h2>
        <p class="text-lg text-gray-600 mb-8 leading-relaxed">
          {description}
        </p>
        <button class="px-6 py-3 rounded-full bg-[#5850ec] text-white font-medium hover:bg-[#4338ca] transition-colors shadow-md mb-12">
          {ctaText}
        </button>

        {#if testimonial}
          <div class="border-t border-gray-100 pt-8 mb-8">
            <blockquote class="text-lg font-medium text-gray-900 mb-6">
              "{testimonial.quote}"
            </blockquote>
            <div class="flex items-center gap-4">
                {#if testimonial.avatar}
                    <img src={testimonial.avatar} alt={testimonial.author} class="w-10 h-10 rounded-full bg-gray-200" />
                {:else}
                    <div class="w-10 h-10 rounded-full bg-gray-200"></div>
                {/if}
              <div>
                <div class="font-bold text-gray-900">{testimonial.author}</div>
                <div class="text-sm text-gray-500">{testimonial.role}</div>
              </div>
              {#if testimonial.readStory}
                <a href="#" class="ml-auto px-3 py-1 rounded-full bg-gray-900 text-white text-xs font-medium hover:bg-gray-800">Read story →</a>
              {/if}
            </div>
          </div>
        {/if}

        {#if stats.length > 0}
          <div class="grid grid-cols-3 gap-8 border-t border-gray-100 pt-8">
            {#each stats as stat}
              <div>
                <div class="text-2xl font-bold text-gray-900">{stat.value}</div>
                <div class="text-xs text-gray-500 mt-1 leading-snug">{stat.label}</div>
              </div>
            {/each}
          </div>
        {/if}
      </div>

      <!-- Image Content -->
      <div class="flex-1 w-full {align === 'left' ? 'lg:order-1' : 'lg:order-2'}">
        <div class="rounded-3xl overflow-hidden aspect-square relative {colorClass} flex items-center justify-center p-8">
            <!-- Pattern -->
            <div class="absolute inset-0 opacity-10" style="background-image: radial-gradient(#000 1px, transparent 1px); background-size: 20px 20px;"></div>
            
            <div class="relative z-10 w-full h-full flex items-center justify-center">
                <slot name="image"></slot>
            </div>
        </div>
      </div>

    </div>
  </div>
</section>
