<div class="relative w-full h-full p-8 flex items-center justify-center">
    <!-- Chart Container -->
    <div class="w-full h-64 bg-[#5850ec] rounded-lg shadow-lg p-4 relative overflow-hidden flex flex-col">
        <!-- Grid Lines -->
        <div class="absolute inset-0 flex flex-col justify-between p-4 opacity-20 pointer-events-none">
            <div class="w-full h-px bg-white"></div>
            <div class="w-full h-px bg-white"></div>
            <div class="w-full h-px bg-white"></div>
            <div class="w-full h-px bg-white"></div>
            <div class="w-full h-px bg-white"></div>
        </div>

        <!-- Bars -->
        <div class="flex-1 flex items-end justify-around gap-2 relative z-10 pt-4">
            <div class="w-8 bg-blue-400/50 rounded-t h-[30%]"></div>
            <div class="w-8 bg-blue-400/50 rounded-t h-[45%]"></div>
            <div class="w-8 bg-blue-400/50 rounded-t h-[40%]"></div>
            <div class="w-8 bg-blue-400/50 rounded-t h-[60%]"></div>
            <div class="w-8 bg-blue-400/50 rounded-t h-[55%]"></div>
            <div class="w-8 bg-white rounded-t h-[85%] shadow-[0_0_10px_rgba(255,255,255,0.5)]"></div>
            <div class="w-8 bg-blue-400/50 rounded-t h-[70%]"></div>
        </div>
        
        <!-- Overlay Line -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none z-20" preserveAspectRatio="none">
            <path d="M20 180 L 70 160 L 120 165 L 170 120 L 220 130 L 270 50 L 320 80" stroke="#34d399" stroke-width="2" fill="none" />
            <circle cx="270" cy="50" r="4" fill="#34d399" stroke="white" stroke-width="2" />
        </svg>
    </div>
</div>
