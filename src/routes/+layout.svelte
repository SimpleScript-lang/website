<script>
    import "../app.css";
  </script>
  
  <header class="flex items-center justify-between whitespace-nowrap border-b border-solid border-b-[#e7edf3] px-10 py-3">
    <div class="flex items-center gap-4 text-[#0e141b]">
      <div class="size-4">
        <svg viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M12.0799 24L4 19.2479L9.95537 8.75216L18.04 13.4961L18.0446 4H29.9554L29.96 13.4961L38.0446 8.75216L44 19.2479L35.92 24L44 28.7521L38.0446 39.2479L29.96 34.5039L29.9554 44H18.0446L18.04 34.5039L9.95537 39.2479L4 28.7521L12.0799 24Z"
            fill="currentColor"
          ></path>
        </svg>
      </div>
      <h2 class="text-[#0e141b] text-lg font-bold leading-tight tracking-[-0.015em]">Simple Script <p class="text-sm font-semibold text-blue-500">beta</p></h2>
    </div>
    <div class="flex flex-1 justify-end gap-8">
      <div class="flex items-center gap-9">
        <a class="text-[#0e141b] text-sm font-medium leading-normal" href="../">Home</a>
        <a class="text-[#0e141b] text-sm font-medium leading-normal" href="/construction">Learn</a>
        <a class="text-[#0e141b] text-sm font-medium leading-normal" href="/codeexamples">Code Examples</a>
        <a class="text-[#0e141b] text-sm font-medium leading-normal" href="/construction">Playground</a>
        <a class="text-[#0e141b] text-sm font-medium leading-normal" href="/construction">Documentation</a>
      </div>
      <div class="flex gap-2">
        <button
          class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-10 px-4 bg-[#1980e6] text-slate-50 text-sm font-bold leading-normal tracking-[0.015em]"
        >
          <a href="/construction" class="truncate">Download</a>
        </button>

      </div>
    </div>
  </header>






  
  <slot />