<script>
  export let transparent = false;
</script>

<nav class="w-full py-4 px-6 md:px-10 flex items-center justify-between sticky top-0 z-50 {transparent ? 'bg-transparent' : 'bg-white/80 backdrop-blur-md'} transition-all duration-300">
  <div class="flex items-center gap-10">
    <a href="/" class="text-2xl font-bold tracking-tight text-gray-900 flex items-center gap-2">
      <!-- Logo Icon -->
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-gray-900">
        <path d="M4 4H20V20H4V4Z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
        <path d="M4 4L20 20" stroke="currentColor" stroke-width="2"/>
      </svg>
      Default
    </a>
    
    <div class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-600">
      <a href="#" class="hover:text-gray-900 flex items-center gap-1">Platform <span class="text-[10px] opacity-50">▼</span></a>
      <a href="#" class="hover:text-gray-900 flex items-center gap-1">Use cases <span class="text-[10px] opacity-50">▼</span></a>
      <a href="#" class="hover:text-gray-900">Pricing</a>
      <a href="#" class="hover:text-gray-900">Resources</a>
    </div>
  </div>

  <div class="flex items-center gap-4 text-sm font-medium">
    <a href="#" class="text-gray-600 hover:text-gray-900 hidden sm:block">Login</a>
    <a href="#" class="bg-[#5850ec] text-white px-4 py-2 rounded-full hover:bg-[#4338ca] transition-colors shadow-sm shadow-indigo-200">Book a demo →</a>
  </div>
</nav>
