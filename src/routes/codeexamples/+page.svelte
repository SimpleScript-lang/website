  <head>
    <link rel="preconnect" href="https://fonts.gstatic.com/" crossorigin="" />
    <link
      rel="stylesheet"
      as="style"
      onload="this.rel='stylesheet'"
      href="https://fonts.googleapis.com/css2?display=swap&amp;family=Noto+Sans%3Awght%40400%3B500%3B700%3B900&amp;family=Space+Grotesk%3Awght%40400%3B500%3B700"
    />
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Source+Code+Pro:ital,wght@0,200..900;1,200..900&display=swap" rel="stylesheet">

    <title>Code Examples | SimpleScript</title>
    <link rel="icon" type="image/x-icon" href="data:image/x-icon;base64," />

    <script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
    <style>
.code-font {
  font-family: "Source Code Pro", monospace;
  font-optical-sizing: auto;
  font-weight: 500;
  font-style: normal;
  color: #FFFFFF;
}
.code-font-desc {
  font-family: "Source Code Pro", monospace;
  font-optical-sizing: auto;
  font-weight: 500;
  font-style: normal;
}
    </style>
  </head>
  <body>
    <div class="relative flex size-full min-h-screen flex-col bg-slate-50 light group/design-root overflow-x-hidden" style='font-family: "Space Grotesk", "Noto Sans", sans-serif;'>
      <div class="layout-container flex h-full grow flex-col">
        <div class="px-40 flex flex-1 justify-center py-5">
          <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
            <div class="flex flex-wrap justify-between gap-3 p-4"><p class="text-black tracking-light text-[32px] font-bold leading-tight min-w-72">Code examples</p></div>
            <h3 class="text-black text-lg font-bold leading-tight tracking-[-0.015em] px-4 pb-2 pt-4">Hello, world!</h3>
            <p class="text-black text-base font-normal leading-normal pb-3 pt-1 px-4">An example of the classic first program in Simple.</p>
            <div class="flex max-w-[480px] flex-wrap items-end gap-4 px-4 py-3">
              <!-- svelte-ignore a11y-label-has-associated-control -->
              <!-- svelte-ignore a11y-label-has-associated-control -->
              <label class="flex flex-col min-w-40 flex-1">
                <div
                  class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-black focus:outline-0 focus:ring-0 border-none bg-[#243647] focus:border-none min-h-36 placeholder:text-[#93adc8] p-4 text-base font-normal leading-normal code-font"
                ><p class="text-yellow-300">print</p> (<p class="text-[#CE834A]">"Hello, World!"</p>)</div>
              </label>
            </div>
            <h3 class="text-black text-lg font-bold leading-tight tracking-[-0.015em] px-4 pb-2 pt-4">Variable Declaration</h3>
            <p class="text-black text-base font-normal leading-normal pb-3 pt-1 px-4">
              Variable declarations have been simplified into just <span class="code-font-desc font-semibold text-[#286ACB]">var</span>, and the variable name! SimpleScript handles the rest
            </p>
            <div class="flex max-w-[480px] flex-wrap items-end gap-0 px-4 py-0">
              <!-- svelte-ignore a11y-label-has-associated-control -->
              <label class="flex flex-col min-w-40 flex-1">
                <div
                class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-black focus:outline-0 focus:ring-0 border-none bg-[#243647] focus:border-none min-h-0 placeholder:text-[#93adc8] p-4 text-base font-normal leading-normal code-font"
                >
                <p class="text-[#286ACB] mr-1">var </p><p class="text-[#9CDCFE] mr-1">name</p> = <p class="text-[#CE9178]">"joshua"</p>
                <br>
print("Hello \name")
              </div>
              </label>
            </div>
          </div>
        </div>
      </div>
    </div>
  </body>