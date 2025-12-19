<script>
  import { onMount } from 'svelte';
</script>

<section class="relative pt-10 pb-20 overflow-hidden bg-gray-50">
  <!-- Dotted Background Pattern -->
  <div class="absolute inset-0 z-0 opacity-[0.4]" style="background-image: radial-gradient(#cbd5e1 1px, transparent 1px); background-size: 24px 24px;"></div>

  <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center text-center">
    
    <!-- Badge -->
    <a href="#" class="inline-flex items-center gap-1 px-3 py-1 rounded-full bg-white border border-gray-200 text-xs font-medium text-gray-600 mb-8 hover:border-gray-300 transition-colors shadow-sm">
      Introducing Default Handoff <span class="text-gray-400">→</span>
    </a>

    <!-- Headline -->
    <h1 class="text-4xl md:text-6xl font-bold tracking-tight text-gray-900 mb-6 max-w-4xl leading-[1.1]">
      Run revenue like an<br/>engineered system
    </h1>

    <!-- Subheadline -->
    <p class="text-lg md:text-xl text-gray-600 mb-10 max-w-2xl leading-relaxed">
      Default is a revenue-grade workflow engine that lets you see your revenue machine, understand how it all connects, and scale without breaking anything.
    </p>

    <!-- Email Input -->
    <div class="flex flex-col sm:flex-row items-center gap-2 mb-16 w-full max-w-lg">
      <input type="email" placeholder="What's your work email?" class="w-full px-4 py-3 rounded-full border border-gray-200 focus:outline-none focus:ring-2 focus:ring-[#5850ec] focus:border-transparent shadow-sm text-sm" />
      <button class="w-full sm:w-auto px-6 py-3 rounded-full bg-[#5850ec] text-white font-medium hover:bg-[#4338ca] transition-colors shadow-md whitespace-nowrap">
        Book a demo →
      </button>
    </div>

    <!-- Logos -->
    <div class="flex flex-wrap justify-center items-center gap-8 md:gap-12 opacity-60 grayscale mb-16">
      <!-- Browserbase -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800"><div class="w-5 h-5 bg-orange-500 rounded-sm"></div>Browserbase</div>
      <!-- Airbyte -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800"><div class="w-5 h-5 bg-blue-400 rounded-full"></div>Airbyte</div>
      <!-- PostHog -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800"><div class="w-5 h-5 bg-yellow-400 rounded-sm"></div>PostHog</div>
      <!-- Justworks -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800">Justworks</div>
      <!-- Plain -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800">Plain</div>
      <!-- rootly -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800"><div class="w-5 h-5 bg-yellow-200 rounded-full"></div>rootly</div>
      <!-- ABTasty -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800"><div class="w-5 h-5 bg-purple-600 rounded-sm"></div>ABTasty</div>
      <!-- lemlist -->
      <div class="h-6 flex items-center gap-2 font-bold text-gray-800"><div class="w-5 h-5 bg-blue-600 rounded-sm"></div>lemlist</div>
    </div>

    <!-- UI Mockup Container -->
    <div class="w-full max-w-6xl bg-white rounded-xl shadow-2xl border border-gray-200 overflow-hidden text-left relative">
      <!-- Toolbar -->
      <div class="h-12 border-b border-gray-100 flex items-center justify-between px-4 bg-white">
        <div class="flex items-center gap-4">
            <div class="flex items-center gap-2 text-sm font-medium text-gray-600">
                <span class="p-1 hover:bg-gray-100 rounded">Workflows</span>
                <span class="text-gray-300">/</span>
                <span class="text-gray-900">Inbound Workflow</span>
            </div>
        </div>
        <div class="flex items-center gap-2">
            <button class="text-sm text-gray-500 px-3 py-1 hover:bg-gray-50 rounded">Share</button>
            <button class="text-sm bg-[#5850ec] text-white px-3 py-1 rounded hover:bg-[#4338ca]">Publish</button>
            <button class="p-1 hover:bg-gray-100 rounded text-gray-400">⋮</button>
        </div>
      </div>

      <div class="flex h-[600px] bg-gray-50/50 relative">
        <!-- Sidebar Icons -->
        <div class="w-12 border-r border-gray-100 bg-white flex flex-col items-center py-4 gap-4">
            {#each Array(8) as _}
                <div class="w-8 h-8 rounded hover:bg-gray-50 flex items-center justify-center text-gray-400 cursor-pointer">
                    <div class="w-4 h-4 border border-current rounded-sm"></div>
                </div>
            {/each}
            <div class="mt-auto w-8 h-8 rounded-full bg-orange-200 overflow-hidden">
                <img src="https://api.dicebear.com/7.x/avataaars/svg?seed=Felix" alt="User" />
            </div>
        </div>

        <!-- Canvas Area -->
        <div class="flex-1 relative overflow-hidden p-8">
            <!-- Background Grid -->
            <div class="absolute inset-0 opacity-[0.3]" style="background-image: radial-gradient(#cbd5e1 1px, transparent 1px); background-size: 20px 20px;"></div>

            <!-- Nodes -->
            
            <!-- Node 1: Form Submission -->
            <div class="absolute top-10 left-1/2 -translate-x-1/2 w-80 bg-white rounded-lg shadow-sm border border-green-200 z-10">
                <div class="p-3 border-b border-gray-50 flex items-center justify-between">
                    <div class="flex items-center gap-2">
                        <div class="w-6 h-6 bg-green-100 rounded flex items-center justify-center text-green-600 text-xs">📝</div>
                        <span class="text-sm font-medium text-gray-900">Form Submission</span>
                    </div>
                    <span class="text-gray-300">•••</span>
                </div>
                <div class="p-3 bg-gray-50/50 rounded-b-lg">
                    <div class="text-xs text-gray-500">Form: <span class="text-blue-500 bg-blue-50 px-1 rounded">Inbound Demo Form</span></div>
                </div>
                <!-- Connection Line Down -->
                <div class="absolute top-full left-1/2 w-px h-8 bg-gray-300"></div>
            </div>

            <!-- Node 2: Enrich with waterfall -->
            <div class="absolute top-40 left-1/2 -translate-x-1/2 w-80 bg-white rounded-lg shadow-sm border border-gray-200 z-10">
                <div class="p-3 border-b border-gray-50 flex items-center justify-between">
                    <div class="flex items-center gap-2">
                        <div class="w-6 h-6 bg-gray-900 rounded flex items-center justify-center text-white text-xs">⚡</div>
                        <span class="text-sm font-medium text-gray-900">Enrich with waterfall</span>
                    </div>
                    <span class="text-gray-300">•••</span>
                </div>
                <div class="p-3">
                    <div class="text-xs font-medium text-gray-500 mb-2">Enrichment Priority:</div>
                    <div class="space-y-1">
                        <div class="flex items-center gap-2 text-xs p-1 bg-yellow-50 border border-yellow-100 rounded">
                            <span class="font-mono text-gray-400">1</span>
                            <div class="w-3 h-3 bg-yellow-400 rounded-full"></div>
                            <span>Apollo.io</span>
                        </div>
                        <div class="flex items-center gap-2 text-xs p-1 bg-white border border-gray-100 rounded">
                            <span class="font-mono text-gray-400">2</span>
                            <div class="w-3 h-3 bg-blue-400 rounded-full"></div>
                            <span>Clearbit</span>
                        </div>
                        <div class="flex items-center gap-2 text-xs p-1 bg-white border border-gray-100 rounded">
                            <span class="font-mono text-gray-400">3</span>
                            <div class="w-3 h-3 bg-red-400 rounded-full"></div>
                            <span>Harmonic</span>
                        </div>
                    </div>
                </div>
                <!-- Connection Line Down -->
                <div class="absolute top-full left-1/2 w-px h-8 bg-gray-300"></div>
            </div>

            <!-- Node 3: Display Scheduler -->
            <div class="absolute top-[340px] left-1/2 -translate-x-1/2 w-80 bg-white rounded-lg shadow-sm border border-gray-200 z-10">
                <div class="p-3 border-b border-gray-50 flex items-center justify-between">
                    <div class="flex items-center gap-2">
                        <div class="w-6 h-6 bg-white border border-gray-200 rounded flex items-center justify-center text-gray-600 text-xs">📅</div>
                        <span class="text-sm font-medium text-gray-900">Display Scheduler</span>
                    </div>
                    <span class="text-gray-300">•••</span>
                </div>
                <div class="p-3 bg-gray-50/50 rounded-b-lg">
                    <div class="text-xs text-gray-500">Meeting Type: <span class="text-blue-500 bg-blue-50 px-1 rounded">30 Minute Demo</span></div>
                </div>
                <!-- Connection Lines Branching -->
                <div class="absolute top-full left-1/2 w-px h-8 bg-gray-300"></div>
                <div class="absolute top-[calc(100%+32px)] left-1/2 -translate-x-1/2 w-[300px] h-px bg-gray-300"></div>
                <div class="absolute top-[calc(100%+32px)] left-[calc(50%-150px)] w-px h-4 bg-gray-300"></div>
                <div class="absolute top-[calc(100%+32px)] left-[calc(50%+150px)] w-px h-4 bg-gray-300"></div>
            </div>

            <!-- Branch Results -->
            <div class="absolute top-[460px] left-[calc(50%-150px)] -translate-x-1/2 px-3 py-1 bg-green-100 text-green-700 text-xs rounded-full font-medium">Meeting booked</div>
            <div class="absolute top-[460px] left-[calc(50%+150px)] -translate-x-1/2 px-3 py-1 bg-red-100 text-red-700 text-xs rounded-full font-medium">Meeting not booked</div>

        </div>

        <!-- Right Panel -->
        <div class="w-64 border-l border-gray-100 bg-white flex flex-col">
            <div class="h-10 border-b border-gray-100 flex items-center justify-between px-3">
                <span class="text-sm font-medium text-gray-900">Objects</span>
                <span class="text-gray-400">×</span>
            </div>
            <div class="flex border-b border-gray-100">
                <button class="flex-1 py-2 text-xs font-medium text-gray-900 border-b-2 border-gray-900">Objects</button>
                <button class="flex-1 py-2 text-xs font-medium text-gray-500">Recipes</button>
            </div>
            <div class="p-3 overflow-y-auto flex-1">
                <div class="text-xs font-medium text-gray-500 mb-2 uppercase tracking-wide">Actions</div>
                <div class="space-y-1 mb-4">
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-blue-100 text-blue-600 flex items-center justify-center text-[10px]">↗</div>
                        <span class="text-xs text-gray-700">Redirect to URL</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-purple-100 text-purple-600 flex items-center justify-center text-[10px]">⚡</div>
                        <span class="text-xs text-gray-700">Webhook</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-gray-100 text-gray-600 flex items-center justify-center text-[10px]">⏱</div>
                        <span class="text-xs text-gray-700">Wait</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-indigo-100 text-indigo-600 flex items-center justify-center text-[10px]">📤</div>
                        <span class="text-xs text-gray-700">Send Data</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                </div>

                <div class="text-xs font-medium text-gray-500 mb-2 uppercase tracking-wide">CRMs</div>
                <div class="space-y-1">
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-blue-50 text-blue-500 flex items-center justify-center text-[10px]">☁</div>
                        <span class="text-xs text-gray-700">Create Record</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-blue-50 text-blue-500 flex items-center justify-center text-[10px]">☁</div>
                        <span class="text-xs text-gray-700">Update Salesforce</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                    <div class="flex items-center gap-2 p-2 hover:bg-gray-50 rounded cursor-pointer border border-transparent hover:border-gray-100 group">
                        <div class="w-5 h-5 rounded bg-orange-50 text-orange-500 flex items-center justify-center text-[10px]">🦊</div>
                        <span class="text-xs text-gray-700">Create Record</span>
                        <span class="ml-auto opacity-0 group-hover:opacity-100 text-gray-300">::</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- Floating Action Buttons on Right Edge -->
        <div class="absolute right-64 top-4 flex flex-col gap-2">
            <button class="w-8 h-8 bg-white rounded shadow-sm border border-gray-200 flex items-center justify-center text-gray-500 hover:text-gray-900">ℹ</button>
            <button class="w-8 h-8 bg-blue-50 rounded shadow-sm border border-blue-200 flex items-center justify-center text-blue-500">✨</button>
            <button class="w-8 h-8 bg-white rounded shadow-sm border border-gray-200 flex items-center justify-center text-gray-500 hover:text-gray-900">🔍</button>
            <button class="w-8 h-8 bg-white rounded shadow-sm border border-gray-200 flex items-center justify-center text-gray-500 hover:text-gray-900">↺</button>
        </div>
      </div>
    </div>
  </div>
</section>
