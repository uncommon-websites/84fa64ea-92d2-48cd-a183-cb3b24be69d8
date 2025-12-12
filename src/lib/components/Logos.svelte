<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-12">
  <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-8">
    <!-- Logos -->
    <div class="flex flex-wrap items-center gap-8 md:gap-12 grayscale opacity-70">
        <!-- Fisher Investments -->
        <div class="h-6 font-bold text-lg tracking-tight">FISHER INVESTMENTS</div>
        <!-- Mercer Advisors -->
        <div class="h-8 flex flex-col leading-none text-xs font-serif uppercase tracking-widest">
            <span>Mercer</span>
            <span>Advisors</span>
        </div>
        <!-- Captrust -->
        <div class="h-6 font-bold text-lg uppercase tracking-wide">CAPTRUST</div>
        <!-- Hightower -->
        <div class="h-6 font-medium text-lg font-serif">
            Hightower
        </div>
    </div>

    <!-- Trust Text -->
    <div class="text-gray-400 text-sm font-light text-right md:text-left">
      Trusted by RIAs managing $500M+
    </div>
  </div>
</SectionWrapper>
