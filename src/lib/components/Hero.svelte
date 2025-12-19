<script>
  let activeTab = 'Order Management';
  const tabs = ['Order Management', 'Compliance', 'Logistics', 'Payments', 'Inventory', 'Reporting', 'Integrations', 'Multi-state', 'Tax & Duty', 'Age Verification'];
</script>

<section class="pt-32 pb-20 px-6 max-w-7xl mx-auto">
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-16">
    <div>
      <h1 class="text-5xl md:text-6xl font-medium tracking-tight text-black leading-[1.1] mb-8">
        Unified infrastructure <br /> for alcohol commerce
      </h1>
    </div>
    <div class="flex flex-col justify-end items-start lg:pl-12">
      <p class="text-xl text-gray-600 mb-6 max-w-md leading-relaxed">
        Integrated compliance, logistics, and payment systems that power the $1.6T alcohol market.
      </p>
      <a href="#" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
        Explore Platform 
        <span class="ml-1 group-hover:translate-x-1 transition-transform">→</span>
      </a>
    </div>
  </div>

  <!-- Interactive Visual Section -->
  <div class="rounded-3xl overflow-hidden bg-gray-50 border border-gray-200 shadow-sm">
    <!-- Tabs -->
    <div class="flex overflow-x-auto scrollbar-hide border-b border-gray-200 bg-white/50 backdrop-blur-sm">
      {#each tabs as tab}
        <button 
          class="px-5 py-4 text-sm font-medium whitespace-nowrap transition-colors relative {activeTab === tab ? 'text-black' : 'text-gray-500 hover:text-gray-800'}"
          on:click={() => activeTab = tab}
        >
          {tab}
          {#if activeTab === tab}
            <div class="absolute bottom-0 left-0 right-0 h-0.5 bg-black"></div>
          {/if}
        </button>
      {/each}
    </div>

    <!-- Content Area -->
    <div class="relative h-[500px] bg-gradient-to-br from-gray-900 to-gray-800 overflow-hidden group">
      <!-- Background Pattern -->
      <div class="absolute inset-0 opacity-10" style="background-image: repeating-linear-gradient(45deg, transparent, transparent 35px, rgba(255,255,255,.05) 35px, rgba(255,255,255,.05) 70px);"></div>
      
      <!-- Floating UI Card -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-80 bg-white/10 backdrop-blur-md border border-white/20 rounded-2xl p-4 text-white shadow-2xl">
        <div class="flex justify-between items-center mb-6">
          <span class="text-xs font-medium text-white/80">Order #ORD-2847</span>
          <span class="px-2 py-1 rounded-full bg-green-500/20 text-green-300 text-[10px] font-medium">Compliant</span>
        </div>
        
        <!-- Order Item 1 -->
        <div class="flex items-center gap-3 mb-4">
          <div class="w-10 h-10 rounded-lg bg-amber-600 flex items-center justify-center text-white shrink-0">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
          </div>
          <div class="flex-1 min-w-0">
            <div class="flex justify-between items-baseline">
              <h3 class="text-sm font-medium truncate">Premium Whiskey</h3>
              <span class="text-sm font-medium">$89.99</span>
            </div>
            <div class="flex justify-between items-baseline">
              <p class="text-xs text-white/60">12 units • CA License</p>
              <p class="text-xs text-white/60">750ml</p>
            </div>
          </div>
        </div>

        <!-- Order Item 2 -->
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 rounded-lg bg-red-700 flex items-center justify-center text-white shrink-0">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
          </div>
          <div class="flex-1 min-w-0">
            <div class="flex justify-between items-baseline">
              <h3 class="text-sm font-medium truncate">Craft Beer Selection</h3>
              <span class="text-sm font-medium">$47.88</span>
            </div>
            <div class="flex justify-between items-baseline">
              <p class="text-xs text-white/60">24 units • Multi-state</p>
              <div class="px-1.5 py-0.5 rounded bg-white/20 text-[10px] font-medium">Verified</div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Code Block -->
    <div class="bg-gray-50 p-6 border-t border-gray-200 overflow-x-auto">
      <pre class="font-mono text-xs leading-relaxed text-gray-600">
<span class="text-gray-400 select-none">1</span>  <span class="text-gray-400"># Create a compliant alcohol order with automatic license verification</span>
<span class="text-gray-400 select-none">2</span>
<span class="text-gray-400 select-none">3</span>  <span class="text-purple-600">curl</span> <span class="text-blue-600">-X POST</span> <span class="text-green-600">'https://api.tipple.com/v1/orders'</span> \
<span class="text-gray-400 select-none">4</span>    <span class="text-blue-600">-H</span> <span class="text-green-600">'Authorization: Bearer YOUR_API_KEY'</span> \
<span class="text-gray-400 select-none">5</span>    <span class="text-blue-600">-H</span> <span class="text-green-600">'Content-Type: application/json'</span> \
<span class="text-gray-400 select-none">6</span>    <span class="text-blue-600">-d</span> '&#123;
<span class="text-gray-400 select-none">7</span>      <span class="text-blue-800">"distributor_id"</span>: <span class="text-green-600">"dist_8f4e2a1b"</span>,
<span class="text-gray-400 select-none">8</span>      <span class="text-blue-800">"retailer_license"</span>: <span class="text-green-600">"CA-ABC-123456"</span>,
<span class="text-gray-400 select-none">9</span>      <span class="text-blue-800">"items"</span>: [&#123;
<span class="text-gray-400 select-none">10</span>       <span class="text-blue-800">"product_id"</span>: <span class="text-green-600">"prod_whiskey_750ml"</span>,
<span class="text-gray-400 select-none">11</span>       <span class="text-blue-800">"quantity"</span>: <span class="text-orange-600">12</span>,
<span class="text-gray-400 select-none">12</span>       <span class="text-blue-800">"compliance_check"</span>: <span class="text-orange-600">true</span></pre>
    </div>
  </div>
</section>
