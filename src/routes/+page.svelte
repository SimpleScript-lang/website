<html lang="eng">
    <head>
        <link rel="preconnect" href="https://fonts.gstatic.com/" crossorigin="" />
        <link
          rel="stylesheet"
          as="style"
          onload="this.rel='stylesheet'"
          href="https://fonts.googleapis.com/css2?display=swap&amp;family=Noto+Sans%3Awght%40400%3B500%3B700%3B900&amp;family=Space+Grotesk%3Awght%40400%3B500%3B700"
        />
        <link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;1,100;1,200;1,300;1,400;1,500;1,600;1,700&display=swap" rel="stylesheet">
    
        <title>SimpleScript</title>
        <link rel="icon" type="image/x-icon" href="data:image/x-icon;base64," />
    
        <script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
        <style>
            span {
  border-right: .05em solid;
  animation: caret 1s steps(1) infinite;
}

@keyframes caret {
  50% {
    border-color: transparent;
  }
}
.ibm-plex-mono-thin {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 100;
  font-style: normal;
}

.ibm-plex-mono-extralight {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 200;
  font-style: normal;
}

.ibm-plex-mono-light {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 300;
  font-style: normal;
}

.ibm-plex-mono-regular {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 400;
  font-style: normal;
}

.ibm-plex-mono-medium {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 500;
  font-style: normal;
}

.ibm-plex-mono-semibold {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 600;
  font-style: normal;
}

.ibm-plex-mono-bold {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 700;
  font-style: normal;
}

.ibm-plex-mono-thin-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 100;
  font-style: italic;
}

.ibm-plex-mono-extralight-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 200;
  font-style: italic;
}

.ibm-plex-mono-light-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 300;
  font-style: italic;
}

.ibm-plex-mono-regular-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 400;
  font-style: italic;
}

.ibm-plex-mono-medium-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 500;
  font-style: italic;
}

.ibm-plex-mono-semibold-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 600;
  font-style: italic;
}

.ibm-plex-mono-bold-italic {
  font-family: "IBM Plex Mono", monospace;
  font-weight: 700;
  font-style: italic;
}

        </style>
       <script>
        document.addEventListener('DOMContentLoaded', function(event) {
          // array with texts to type in typewriter
          var dataText = ["Simple ", "Extendable ", "Teachable ", "Powerful ", "Lightweight ", "User-friendly ", "Modern ", "Innovative "];
        
          // type one text in the typewriter
          // keeps calling itself until the text is finished
          function typeWriter(text, i, fnCallback) {
            // check if text isn't finished yet
            if (i < text.length) {
              // add next character to h1
              document.getElementById("scrollType").innerHTML = text.substring(0, i + 1) + '<span aria-hidden="true"></span>';
        
              // wait for a while and call this function again for next character
              setTimeout(function() {
                typeWriter(text, i + 1, fnCallback);
              }, 100);
            }
            // text finished, call callback if there is a callback function
            else if (typeof fnCallback === 'function') {
              // call callback after timeout
              setTimeout(fnCallback, 700);
            }
          }
        
          // start a typewriter animation for a text in the dataText array
          function StartTextAnimation(i) {
            if (typeof dataText[i] === 'undefined') {
              setTimeout(function() {
                StartTextAnimation(0);
              }, 20000);
            } else if (i < dataText.length) {
              // text exists! start typewriter animation
              typeWriter(dataText[i], 0, function() {
                // after callback (and whole text has been animated), start next text
                StartTextAnimation(i + 1);
              });
            }
          }
        
          // start the text animation
          StartTextAnimation(0);
        });
        </script>
    </head>
    <body>

    <div class="relative flex size-full min-h-screen flex-col bg-slate-50 group/design-root overflow-x-hidden" style='font-family: "Space Grotesk", "Noto Sans", sans-serif;'>

        <div class="layout-container flex h-full grow flex-col">

          <div class="px-60 flex flex-1 justify-center py-5">
            <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
              <div class="@container">
                <div class="@[480px]:p-4">
                  <div
                    class="flex min-h-[0px] flex-col gap-6 bg-cover bg-center bg-no-repeat @[0px]:gap-8 @[480px]:rounded-xl items-start justify-end px-4 pb-1 @[480px]:px-10"> 
                  <h1
                      class="text-black text-4xl font-black leading-tight tracking-[-0.033em] @[480px]:text-5xl @[480px]:font-black @[480px]:leading-tight @[480px]:tracking-[-0.033em] text-center pl-50"
                    >
                    SimpleScript is <span id="scrollType" class="text-blue-900 font-extrabold">loading...</span>
                  </h1>
                  </div>
                </div>
              </div>
              <div class="flex flex-col gap-10 px-4 py-10 @container">
                <div class="flex flex-col gap-4">
                  <p class="text-[#0e141b] text-base font-normal text-xl leading-normal max-w-[720px] text-center">
                    <!-- svelte-ignore a11y-missing-attribute -->
                    Simple Script is a <a class="font-semibold text-green-600">beginner-friendly</a> coding language that makes it easy to <a class="font-semibold text-red-600">learn</a>, <a class="font-semibold text-blue-600">write</a>, and <a class="font-semibold text-purple-600">share code</a>. It's perfect for beginners, students, and educators who
                    want to learn or teach programming. Save <b>simplescript.co</b> for more!
                  </p>
                </div>
                <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3">
                  <div class="flex flex-col gap-3 pb-3">
                    <div
                      class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                      style='background-image: url("https://cdn.usegalileo.ai/stability/c4df0bfb-8693-4875-b2ce-1a867616d0a4.png");'
                    ></div>
                    <div>
                      <p class="text-[#0e141b] text-base font-medium leading-normal">Learn</p>
                      <p class="text-[#4e7397] text-sm font-normal leading-normal">Simple Script is super easy for new coders to learn</p>
                    </div>
                  </div>
                  <div class="flex flex-col gap-3 pb-3">
                    <div
                      class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                      style='background-image: url("https://cdn.usegalileo.ai/stability/e1d85c94-22f7-4396-96e3-1369415cbe12.png");'
                    ></div>
                    <div>
                      <p class="text-[#0e141b] text-base font-medium leading-normal">Write</p>
                      <p class="text-[#4e7397] text-sm font-normal leading-normal">Write simple code in the online interactive editor, or in any editor of your choice!</p>
                    </div>
                  </div>
                  <div class="flex flex-col gap-3 pb-3">
                    <div
                      class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                      style='background-image: url("https://cdn.usegalileo.ai/stability/b63e1bdd-c498-4962-82f2-dacea539702a.png");'
                    ></div>
                    <div>
                      <p class="text-[#0e141b] text-base font-medium leading-normal">Share</p>
                      <p class="text-[#4e7397] text-sm font-normal leading-normal">Share your code with friends and build the future of computer projects</p>
                    </div>
                  </div>
                </div>
              </div>
              
              <div class="flex px-4 py-3 justify-end">
              </div>
              <h2 class="text-[#0e141b] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">Documentation &amp; Community</h2>
              <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
                <div class="flex flex-1 gap-3 rounded-lg border border-[#d0dbe7] bg-slate-50 p-4 flex-col">
                  <div class="text-[#0e141b]" data-icon="Book" data-size="24px" data-weight="regular">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                      <path
                        d="M208,24H72A32,32,0,0,0,40,56V224a8,8,0,0,0,8,8H192a8,8,0,0,0,0-16H56a16,16,0,0,1,16-16H208a8,8,0,0,0,8-8V32A8,8,0,0,0,208,24Zm-8,160H72a31.82,31.82,0,0,0-16,4.29V56A16,16,0,0,1,72,40H200Z"
                      ></path>
                    </svg>
                  </div>
                  <div class="flex flex-col gap-1">
                    <h2 class="text-[#0e141b] text-base font-bold leading-tight">Docs</h2>
                    <p class="text-[#4e7397] text-sm font-normal leading-normal">Learn Simple Script with our official documentation</p>
                  </div>
                </div>
                <div class="flex flex-1 gap-3 rounded-lg border border-[#d0dbe7] bg-slate-50 p-4 flex-col">
                  <div class="text-[#0e141b]" data-icon="Users" data-size="24px" data-weight="regular">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                      <path
                        d="M117.25,157.92a60,60,0,1,0-66.5,0A95.83,95.83,0,0,0,3.53,195.63a8,8,0,1,0,13.4,8.74,80,80,0,0,1,134.14,0,8,8,0,0,0,13.4-8.74A95.83,95.83,0,0,0,117.25,157.92ZM40,108a44,44,0,1,1,44,44A44.05,44.05,0,0,1,40,108Zm210.14,98.7a8,8,0,0,1-11.07-2.33A79.83,79.83,0,0,0,172,168a8,8,0,0,1,0-16,44,44,0,1,0-16.34-84.87,8,8,0,1,1-5.94-14.85,60,60,0,0,1,55.53,105.64,95.83,95.83,0,0,1,47.22,37.71A8,8,0,0,1,250.14,206.7Z"
                      ></path>
                    </svg>
                  </div>
                  <div class="flex flex-col gap-1">
                    <h2 class="text-[#0e141b] text-base font-bold leading-tight">Community</h2>
                    <p class="text-[#4e7397] text-sm font-normal leading-normal">Join the Simple Script community for help and inspiration</p>
                  </div>
                </div>
                <div class="flex flex-1 gap-3 rounded-lg border border-[#d0dbe7] bg-slate-50 p-4 flex-col">
                  <div class="text-[#0e141b]" data-icon="Question" data-size="24px" data-weight="regular">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                      <path
                        d="M140,180a12,12,0,1,1-12-12A12,12,0,0,1,140,180ZM128,72c-22.06,0-40,16.15-40,36v4a8,8,0,0,0,16,0v-4c0-11,10.77-20,24-20s24,9,24,20-10.77,20-24,20a8,8,0,0,0-8,8v8a8,8,0,0,0,16,0v-.72c18.24-3.35,32-17.9,32-35.28C168,88.15,150.06,72,128,72Zm104,56A104,104,0,1,1,128,24,104.11,104.11,0,0,1,232,128Zm-16,0a88,88,0,1,0-88,88A88.1,88.1,0,0,0,216,128Z"
                      ></path>
                    </svg>
                  </div>
                  <div class="flex flex-col gap-1">
                    <h2 class="text-[#0e141b] text-base font-bold leading-tight">FAQ</h2>
                    <p class="text-[#4e7397] text-sm font-normal leading-normal">Find answers to common questions about Simple Script</p>
                  </div>
                </div>
                <div class="flex flex-1 gap-3 rounded-lg border border-[#d0dbe7] bg-slate-50 p-4 flex-col">
                  <div class="text-[#0e141b]" data-icon="ChatTeardropText" data-size="24px" data-weight="regular">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                      <path
                        d="M168,112a8,8,0,0,1-8,8H96a8,8,0,0,1,0-16h64A8,8,0,0,1,168,112Zm-8,24H96a8,8,0,0,0,0,16h64a8,8,0,0,0,0-16Zm72-12A100.11,100.11,0,0,1,132,224H47.67A15.69,15.69,0,0,1,32,208.33V124a100,100,0,0,1,200,0Zm-16,0a84,84,0,0,0-168,0v84h84A84.09,84.09,0,0,0,216,124Z"
                      ></path>
                    </svg>
                  </div>
                  <div class="flex flex-col gap-1">
                    <h2 class="text-[#0e141b] text-base font-bold leading-tight">Discussions</h2>
                    <p class="text-[#4e7397] text-sm font-normal leading-normal">Discuss Simple Script with other users and the team</p>
                  </div>
                </div>
                
              </div>
              <div class="pt-10 flex flex-col items-center justify-cente rounded-md bg-gradient-to-r from-blue-400 to-indigo-400">
                <h2 class="text-4xl font-bold">Find code examples</h2>
                <p class="p-3">See how Simple Script truely works in the real world</p>
                <a class="bg-[#1980e6] rounded-md p-4 pb-4 font-semibold mb-6" href='/codeexamples'>
                  Code Examples
                </a>
                </div>
            </div>
            
          </div>
        </div>
      </div>
    </body>
</html>
