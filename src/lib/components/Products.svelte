<script>
  // No script needed
</script>

<div class="space-y-32 pb-32">
  <!-- Order Management Section -->
  <section class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div>
      <h3 class="text-4xl font-medium mb-6">Order Management</h3>
      <p class="text-xl text-gray-600 mb-8 leading-relaxed">
        <strong class="text-black">Unified order orchestration.</strong> One API to manage orders across distributors, retailers, and fulfillment—with built-in compliance checks and real-time inventory sync.
      </p>
      <div class="flex flex-col gap-2">
        <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
          Learn more 
          <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
        </a>
        <a href="#" class="text-sm text-gray-400 hover:text-black transition-colors">View docs</a>
      </div>
    </div>
    <div class="bg-gray-50 rounded-3xl p-12 flex items-center justify-center min-h-[400px]">
      <!-- Order Flow Visualization -->
      <div class="relative w-full max-w-md">
        <div class="flex justify-between items-center">
          <!-- Central Hub -->
          <div class="w-16 h-16 bg-black rounded-lg flex items-center justify-center relative z-10">
            <svg width="32" height="32" viewBox="0 0 24 24" fill="white"><path d="M3 3h7v7H3V3zm11 0h7v7h-7V3zm0 11h7v7h-7v-7zM3 14h7v7H3v-7z"/></svg>
          </div>
          
          <!-- Endpoints -->
          <div class="flex flex-col gap-3">
            {#each ['Orders', 'Compliance', 'Inventory', 'Fulfillment', 'Payments', 'Tracking', 'Returns'] as item, i}
              <div class="flex items-center gap-4">
                <div class="w-24 h-[1px] bg-gradient-to-r from-black/20 to-transparent transform rotate-180 origin-left"></div>
                <div class="flex items-center gap-2">
                  <div class="w-3 h-3 rounded-full" style="background-color: hsl({i * 50}, 70%, 50%)"></div>
                  <span class="text-xs font-medium text-gray-600">{item}</span>
                </div>
              </div>
            {/each}
          </div>
        </div>
        <!-- Connecting lines (simplified) -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none" style="z-index: 0;">
          <defs>
            <linearGradient id="lineGradient" x1="0%" y1="0%" x2="100%" y2="0%">
              <stop offset="0%" stop-color="#000" stop-opacity="0.1" />
              <stop offset="100%" stop-color="#000" stop-opacity="0" />
            </linearGradient>
          </defs>
          <!-- Curved lines would go here, but using straight CSS lines above for simplicity -->
        </svg>
      </div>
    </div>
  </section>

  <!-- Compliance Section -->
  <section class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div>
      <h3 class="text-4xl font-medium mb-6">Compliance Engine</h3>
      <p class="text-xl text-gray-600 mb-8 leading-relaxed">
        <strong class="text-black">Automated regulatory compliance.</strong> Tipple handles license verification, age checks, state regulations, and tax calculations—so your team can focus on growth, not paperwork.
      </p>
      <div class="flex flex-col gap-2">
        <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
          Learn more 
          <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
        </a>
        <a href="#" class="text-sm text-gray-400 hover:text-black transition-colors">View docs</a>
      </div>
    </div>
    <div class="bg-[#E8F5E9] rounded-3xl overflow-hidden min-h-[400px] relative">
      <div class="absolute inset-0 p-8 font-mono text-xs leading-none text-[#4CAF50] opacity-50 break-all overflow-hidden select-none">
        {Array(2000).fill(0).map(() => Math.random().toString(36).substring(2, 3)).join('')}
      </div>
      <div class="absolute inset-0 bg-gradient-to-b from-transparent to-[#E8F5E9]"></div>
    </div>
  </section>

  <!-- ERP Integrations Section -->
  <section class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
    <div>
      <h3 class="text-4xl font-medium mb-6">ERP Connectors</h3>
      <p class="text-xl text-gray-600 mb-8 leading-relaxed">
        <strong class="text-black">Pre-built integrations.</strong> Connect to existing ERP systems with zero custom development. Sync inventory, orders, and financials in real-time across your entire operation.
      </p>
      <div class="flex flex-col gap-2">
        <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
          Learn more 
          <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
        </a>
        <a href="#" class="text-sm text-gray-400 hover:text-black transition-colors">View docs</a>
      </div>
    </div>
    <div class="bg-black rounded-3xl p-12 flex items-center justify-center min-h-[400px]">
      <!-- Dashboard Mockup -->
      <div class="relative w-full max-w-md bg-gray-900 rounded-2xl border border-gray-800 shadow-2xl overflow-hidden">
        <!-- Screen Content -->
        <div class="bg-gray-900 p-6 text-white">
          <div class="flex justify-between items-center mb-6">
            <span class="text-sm font-medium">Connected Systems</span>
            <div class="px-2 py-1 rounded-full bg-green-500/20 text-green-400 text-[10px] font-medium">All Active</div>
          </div>
          <div class="space-y-3">
             <div class="bg-gray-800/50 p-4 rounded-xl flex items-center gap-3 border border-gray-700">
               <div class="w-10 h-10 rounded-lg bg-blue-600 flex items-center justify-center text-white font-bold text-xs">SAP</div>
               <div class="flex-1">
                 <div class="text-sm font-medium">SAP Business One</div>
                 <div class="text-[10px] text-gray-400">Last sync: 2 min ago</div>
               </div>
               <div class="w-2 h-2 rounded-full bg-green-400"></div>
             </div>
             <div class="bg-gray-800/50 p-4 rounded-xl flex items-center gap-3 border border-gray-700">
               <div class="w-10 h-10 rounded-lg bg-orange-600 flex items-center justify-center text-white font-bold text-xs">NS</div>
               <div class="flex-1">
                 <div class="text-sm font-medium">NetSuite</div>
                 <div class="text-[10px] text-gray-400">Last sync: 5 min ago</div>
               </div>
               <div class="w-2 h-2 rounded-full bg-green-400"></div>
             </div>
             <div class="bg-gray-800/50 p-4 rounded-xl flex items-center gap-3 border border-gray-700">
               <div class="w-10 h-10 rounded-lg bg-purple-600 flex items-center justify-center text-white font-bold text-xs">QBO</div>
               <div class="flex-1">
                 <div class="text-sm font-medium">QuickBooks</div>
                 <div class="text-[10px] text-gray-400">Last sync: 1 min ago</div>
               </div>
               <div class="w-2 h-2 rounded-full bg-green-400"></div>
             </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</div>
