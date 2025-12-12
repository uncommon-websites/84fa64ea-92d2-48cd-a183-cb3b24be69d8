<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
  import SolutionBlock from './SolutionBlock.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="">
  <div class="px-4 md:px-12">
    <div class="py-16 text-center">
      <h2 class="font-serif text-4xl text-gray-900">How Glynac works</h2>
    </div>

    <!-- Block 1 -->
    <SolutionBlock
      label="Unified Data Intelligence"
      title="Connect all your systems"
      description="Glynac integrates seamlessly with your CRM, portfolio management, custodian platforms, and document systems. No more switching between tabs or hunting for client information across multiple logins."
    >
      <!-- Visual for Block 1: Files -->
      <div class="relative w-full h-full flex items-center justify-center">
        <!-- Central Hub -->
        <div class="w-16 h-16 bg-white shadow-lg rounded-lg flex items-center justify-center z-10 border border-gray-100">
           <div class="w-8 h-8 bg-gray-900 rounded-sm"></div>
        </div>
        
        <!-- Connected Systems -->
        <div class="absolute top-1/4 left-1/4 bg-white p-3 shadow rounded border border-gray-100 animate-pulse">
            <div class="w-8 h-10 bg-teal-100 rounded flex items-center justify-center text-[10px] font-bold text-teal-700">CRM</div>
            <div class="mt-1 text-[10px] text-center">Salesforce</div>
        </div>
        <div class="absolute top-1/4 right-1/4 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-800 rounded flex items-center justify-center text-[10px] font-bold text-white">PMS</div>
            <div class="mt-1 text-[10px] text-center">Orion</div>
        </div>
        <div class="absolute bottom-1/4 left-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-600 rounded flex items-center justify-center text-[10px] font-bold text-white">DOC</div>
            <div class="mt-1 text-[10px] text-center">Laserfiche</div>
        </div>
         <div class="absolute bottom-1/4 right-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-300 rounded flex items-center justify-center text-[10px] font-bold text-gray-700">CUST</div>
            <div class="mt-1 text-[10px] text-center">Schwab</div>
        </div>
        
        <!-- Connecting Lines (Simplified) -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-20" viewBox="0 0 400 300">
            <path d="M100 100 L200 150 M300 100 L200 150 M150 220 L200 150 M250 220 L200 150" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
        </svg>
      </div>
    </SolutionBlock>

    <!-- Block 2 -->
    <SolutionBlock
      label="Natural Language Queries"
      title="Ask questions, get instant answers"
      description="Simply type or speak your questions in plain English. 'What's the Johnson family's asset allocation?' 'Show me all clients with upcoming reviews.' Glynac understands context and delivers precise answers in seconds, not minutes."
      reversed={true}
    >
      <!-- Visual for Block 2: Query Interface -->
      <div class="bg-white rounded-lg shadow-xl p-6 w-3/4 max-w-sm border border-gray-100">
        <div class="flex items-center space-x-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-gray-900 flex items-center justify-center text-white text-xs font-bold">
                AI
            </div>
            <div class="text-xs text-gray-500">Glynac AI Assistant</div>
        </div>
        <h4 class="font-serif text-xl mb-4">Query Results</h4>
        <div class="space-y-2 mb-6">
            <div class="h-2 bg-gray-100 rounded w-full"></div>
            <div class="h-2 bg-gray-100 rounded w-5/6"></div>
            <div class="h-2 bg-gray-100 rounded w-4/6"></div>
        </div>
        <button class="w-full bg-gray-900 text-white py-2 rounded text-sm font-medium flex items-center justify-center space-x-2">
            <span>View Full Details</span>
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
        </button>
      </div>
    </SolutionBlock>

    <!-- Block 3 -->
    <SolutionBlock
      label="Time Savings Analytics"
      title="Reclaim 40% of your time"
      description="Track exactly how much time Glynac saves your team. From eliminating system switching to instant data retrieval, see the productivity gains in real-time. Focus on what matters: building client relationships and growing your practice."
    >
       <!-- Visual for Block 3: Analytics Dashboard -->
       <div class="bg-white rounded shadow-lg p-8 w-2/3 max-w-xs border border-gray-100 relative">
          <div class="flex justify-between items-center mb-6 border-b pb-2">
              <div class="font-bold text-xs">Time Saved This Month</div>
              <div class="w-4 h-4 bg-gray-900 rounded-full"></div>
          </div>
          <div class="mb-4">
              <h5 class="font-bold text-3xl">156 hrs</h5>
              <div class="text-[10px] text-gray-400">Across 8 advisors using Glynac</div>
          </div>
          <div class="space-y-2 text-[8px] text-gray-500 leading-relaxed">
              <p>• 89 hrs saved on data retrieval</p>
              <p>• 42 hrs saved on report generation</p>
              <p>• 25 hrs saved on system navigation</p>
          </div>
       </div>
    </SolutionBlock>
  </div>
</SectionWrapper>
