<script>
  let activeTab = 'HVAC Services';
  const tabs = ['HVAC Services', 'Plumbing', 'Electrical', 'Landscaping', 'Cleaning', 'Property Mgmt', 'Auto Repair', 'Home Services'];
</script>

<section class="pt-32 pb-20 px-6 max-w-7xl mx-auto">
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-16">
    <div>
      <h1 class="text-5xl md:text-6xl font-medium tracking-tight text-black leading-[1.1] mb-8">
        Modernizing Essential Services Through AI
      </h1>
    </div>
    <div class="flex flex-col justify-end items-start lg:pl-12">
      <p class="text-xl text-gray-600 mb-6 max-w-md leading-relaxed">
        We acquire and transform service businesses with AI-driven automation, delivering stable cash flows and venture-scale returns.
      </p>
      <a href="#approach" class="group inline-flex items-center text-black font-medium hover:opacity-70 transition-opacity">
        Our Approach 
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
    <div class="relative h-[500px] bg-gradient-to-br from-gray-100 to-gray-200 overflow-hidden group">
      <!-- Background Pattern -->
      <div class="absolute inset-0 opacity-30" style="background-image: linear-gradient(rgba(0,0,0,0.05) 1px, transparent 1px), linear-gradient(90deg, rgba(0,0,0,0.05) 1px, transparent 1px); background-size: 40px 40px;"></div>
      
      <!-- Floating Dashboard Card -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[500px] bg-white border border-gray-200 rounded-2xl p-6 shadow-2xl">
        <div class="flex justify-between items-center mb-6">
          <span class="text-sm font-semibold text-black">Operations Dashboard</span>
          <span class="text-xs text-gray-500">Real-time AI Optimization</span>
        </div>
        
        <!-- Metric Cards -->
        <div class="grid grid-cols-3 gap-3 mb-6">
          <div class="bg-gray-50 rounded-lg p-3">
            <div class="text-xs text-gray-500 mb-1">EBITDA Margin</div>
            <div class="text-xl font-bold text-black">32%</div>
            <div class="text-xs text-green-600 font-medium">↑ 12% YoY</div>
          </div>
          <div class="bg-gray-50 rounded-lg p-3">
            <div class="text-xs text-gray-500 mb-1">Labor Cost</div>
            <div class="text-xl font-bold text-black">-18%</div>
            <div class="text-xs text-green-600 font-medium">↓ Automated</div>
          </div>
          <div class="bg-gray-50 rounded-lg p-3">
            <div class="text-xs text-gray-500 mb-1">Jobs/Day</div>
            <div class="text-xl font-bold text-black">147</div>
            <div class="text-xs text-green-600 font-medium">↑ 34%</div>
          </div>
        </div>

        <!-- AI Activity Feed -->
        <div class="space-y-3">
          <div class="flex items-start gap-3 p-3 bg-blue-50 rounded-lg border border-blue-100">
            <div class="w-8 h-8 rounded-full bg-blue-500 flex items-center justify-center text-white shrink-0 text-xs font-bold">AI</div>
            <div class="flex-1 min-w-0">
              <div class="text-sm font-medium text-black">Route optimization completed</div>
              <div class="text-xs text-gray-600">Saved 2.3 hours across 12 service calls</div>
            </div>
            <span class="text-xs text-gray-500">2m ago</span>
          </div>

          <div class="flex items-start gap-3 p-3 bg-green-50 rounded-lg border border-green-100">
            <div class="w-8 h-8 rounded-full bg-green-500 flex items-center justify-center text-white shrink-0 text-xs font-bold">AI</div>
            <div class="flex-1 min-w-0">
              <div class="text-sm font-medium text-black">Dispatch automation active</div>
              <div class="text-xs text-gray-600">8 jobs auto-assigned to optimal technicians</div>
            </div>
            <span class="text-xs text-gray-500">8m ago</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Metrics Bar -->
    <div class="bg-gray-50 p-6 border-t border-gray-200">
      <div class="grid grid-cols-4 gap-6 text-center">
        <div>
          <div class="text-2xl font-bold text-black mb-1">$2T</div>
          <div class="text-xs text-gray-600">Physical Economy TAM</div>
        </div>
        <div>
          <div class="text-2xl font-bold text-black mb-1">25-35%</div>
          <div class="text-xs text-gray-600">Target EBITDA Margins</div>
        </div>
        <div>
          <div class="text-2xl font-bold text-black mb-1">3-5x</div>
          <div class="text-xs text-gray-600">AI-Driven Multiple Expansion</div>
        </div>
        <div>
          <div class="text-2xl font-bold text-black mb-1">12-18mo</div>
          <div class="text-xs text-gray-600">Modernization Timeline</div>
        </div>
      </div>
    </div>
  </div>
</section>
