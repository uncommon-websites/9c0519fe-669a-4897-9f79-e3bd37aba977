<script lang="ts">
</script>

<section class="relative h-screen min-h-[800px] w-full overflow-hidden bg-[#8C8C84]">
    <!-- Background Image -->
    <div class="absolute inset-0 w-full h-full">
        <img 
            src="https://images.unsplash.com/photo-1518531933037-91b2f5f229cc?q=80&w=2000&auto=format&fit=crop" 
            alt="Nature background" 
            class="w-full h-full object-cover opacity-90"
        />
        <div class="absolute inset-0 bg-black/10"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 h-full container mx-auto px-6 md:px-12 flex items-center">
        <div class="w-full grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <!-- Left Text -->
            <div class="text-white max-w-xl">
                <span class="inline-block text-[10px] font-bold tracking-widest uppercase mb-6 opacity-80">
                    ● LCV®
                </span>
                
                <h2 class="text-4xl md:text-[56px] leading-[1.1] font-medium tracking-tight mb-12">
                    Most probiotics don't survive digestion—DS-01® does.
                </h2>
                
                <div class="flex items-center gap-6 bg-white/10 backdrop-blur-md p-6 rounded-lg max-w-md border border-white/10">
                    <div class="flex flex-col">
                        <span class="text-[10px] uppercase tracking-widest opacity-70 mb-1">DS-01® Increases</span>
                        <span class="text-sm font-medium">healthy bacteria by</span>
                    </div>
                    <div class="text-5xl font-light tracking-tighter">
                        3.1x<sup class="text-lg">*</sup>
                    </div>
                    <div class="ml-auto">
                        <div class="w-8 h-8 rounded-full border border-white/30 flex items-center justify-center">
                            <svg width="10" height="10" viewBox="0 0 10 10" fill="currentColor" class="transform rotate-[-45deg]">
                                <path d="M5 0L5 10M0 5L10 5" stroke="currentColor" stroke-width="1.5" />
                            </svg>
                        </div>
                    </div>
                </div>
                
                <p class="mt-8 text-[10px] opacity-60 max-w-xs">
                    *in a clinical trial of n=103 individuals with occasional GI challenges
                </p>
            </div>

            <!-- Right Capsule Diagram -->
            <div class="relative h-[600px] flex items-center justify-center">
                <!-- Capsule Container -->
                <div class="relative w-32 h-96">
                    <!-- Outer Capsule (Top) -->
                    <div class="absolute top-0 w-full h-[55%] bg-green-700/40 backdrop-blur-sm rounded-t-full border-t border-l border-r border-white/30 z-20 shadow-[inset_0_0_20px_rgba(255,255,255,0.2)]"></div>
                    <!-- Outer Capsule (Bottom) -->
                    <div class="absolute bottom-0 w-full h-[55%] bg-green-700/40 backdrop-blur-sm rounded-b-full border-b border-l border-r border-white/30 z-20 shadow-[inset_0_0_20px_rgba(255,255,255,0.2)]"></div>
                    
                    <!-- Inner Capsule -->
                    <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-20 h-64 z-10">
                         <div class="w-full h-1/2 bg-[#D4E995] rounded-t-full opacity-90"></div>
                         <div class="w-full h-1/2 bg-[#C0D888] rounded-b-full opacity-90"></div>
                         <!-- Powder effect -->
                         <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-32 h-32 bg-[#D4E995] blur-xl opacity-20"></div>
                    </div>
                    
                    <!-- Labels -->
                    <div class="absolute top-[20%] -left-48 text-right w-40 hidden md:block">
                        <h4 class="text-[10px] font-bold uppercase tracking-widest text-white mb-1">Outer Capsule</h4>
                        <p class="text-[10px] text-white/70 leading-relaxed">
                            Shields probiotics from stomach acid in the digestive tract, while delivering prebiotics to stimulate the growth of beneficial bacteria.
                        </p>
                        <div class="absolute top-2 -right-6 w-6 h-[1px] bg-white/30"></div>
                    </div>
                    
                    <div class="absolute bottom-[20%] -right-48 text-left w-40 hidden md:block">
                        <h4 class="text-[10px] font-bold uppercase tracking-widest text-white mb-1">Inner Capsule</h4>
                        <p class="text-[10px] text-white/70 leading-relaxed">
                            Delivers 24 live strains of probiotics to the colon, where they're needed most.
                        </p>
                        <div class="absolute top-2 -left-6 w-6 h-[1px] bg-white/30"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
