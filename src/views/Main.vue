<template>
  <!-- This example requires Tailwind CSS v2.0+ -->
  <div class="h-screen flex overflow-hidden bg-white">
    <!-- Static sidebar for desktop -->
    <div class="hidden lg:flex lg:flex-shrink-0">
      <div class="flex flex-col w-64">
        <!-- Sidebar component, swap this element with another sidebar if you like -->
        <div class="flex flex-col h-0 flex-1 border-r border-gray-200 bg-gray-100">
          <div class="flex-1 flex flex-col pt-4 pb-2 overflow-y-auto">
            <div class="flex items-center flex-shrink-0 px-2">
              <svg
                class="h-8 w-auto"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 528.35 128.02"
              ><defs><linearGradient
                id="a"
                x1="60.36"
                y1="120.71"
                x2="60.36"
                gradientUnits="userSpaceOnUse"
              ><stop
                offset="0"
                stop-color="#ffd53f"
              /><stop
                offset=".06"
                stop-color="#eed64e"
              /><stop
                offset=".32"
                stop-color="#a6db8c"
              /><stop
                offset=".55"
                stop-color="#6ddebe"
              /><stop
                offset=".75"
                stop-color="#44e1e1"
              /><stop
                offset=".91"
                stop-color="#2be2f7"
              /><stop
                offset="1"
                stop-color="#22e3ff"
              /></linearGradient><linearGradient
                id="b"
                x1="65.93"
                y1="21.5"
                x2="70.75"
                y2="128.94"
                gradientUnits="userSpaceOnUse"
              ><stop
                offset=".06"
                stop-color="#566690"
              /><stop
                offset=".54"
                stop-color="#00293e"
              /><stop
                offset=".7"
                stop-color="#001723"
              /><stop
                offset=".89"
                stop-color="#000609"
              /><stop offset="1" /></linearGradient></defs><g data-name="Layer 2"><g data-name="Layer 1"><path
                id="logo-name"
                d="M170 75.32v42.76h-13.09V17.54h26.86q13.14 0 19.35 2.69a20.61 20.61 0 0 1 9.6 8.12 21.63 21.63 0 0 1 3.4 11.71 32.4 32.4 0 0 1-2.26 11.71 35.65 35.65 0 0 1-6.24 10.52 41.18 41.18 0 0 1-11.47 8.77l29.08 47h-15.59L183 75.32zm0-10h18.27a32.61 32.61 0 0 0 9.17-6.87 25.89 25.89 0 0 0 4.56-7.51 21.43 21.43 0 0 0 1.56-7.94 13.77 13.77 0 0 0-5.14-11.25q-5.14-4.18-18.66-4.19H170zM281.58 101.89a38.86 38.86 0 0 1-13.25 13.62q-7.74 4.58-14.22 4.58-9.08 0-16.3-7.84t-7.22-23.78a50.7 50.7 0 0 1 4.8-22.47 40.25 40.25 0 0 1 12.84-15.61q8-5.74 19.91-5.74 3.44 0 10.35.72c.69.08 1.72.19 3.1.32h12.09v51.1q0 13.1 2.79 21.26H283.9a110.53 110.53 0 0 1-2.32-16.16zm.05-14.41V56.41a47.39 47.39 0 0 0-11.94-1.69 23.54 23.54 0 0 0-18.59 8.63q-7.42 8.62-7.43 23.48 0 10.77 4.06 16.24t9.24 5.49q5.65 0 12.47-5.71a54.38 54.38 0 0 0 12.19-15.37zM336.24 118.08L304.8 45.72H318l24.84 57.33 25.25-57.33h12.1l-31.69 72.36zM448.6 113.27q-14.44 6.81-27.33 6.82a32.12 32.12 0 0 1-17.5-4.86 34.61 34.61 0 0 1-12.33-13.88A41.71 41.71 0 0 1 386.8 82a43.25 43.25 0 0 1 4.41-19 34 34 0 0 1 12.31-14.21 31.93 31.93 0 0 1 17.62-5.08q12.89 0 20.7 9.18t7.8 28.33v2.59h-49.88a30.11 30.11 0 0 0 3.14 13.77 22.46 22.46 0 0 0 8.26 9.35 22 22 0 0 0 11.66 3.12q11.65 0 25.78-7.8zm-48.13-38.46h36.08v-1.75q0-8.85-4.34-14.08a14.3 14.3 0 0 0-11.59-5.23A17.37 17.37 0 0 0 408 59.08q-5.39 5.33-7.53 15.73zM468 118.08V45.72h12v15.81a40.73 40.73 0 0 1 12.5-13.09 26.83 26.83 0 0 1 14.64-4.73 21.06 21.06 0 0 1 11.66 3.4 18.18 18.18 0 0 1 7.44 8.89q2.1 5.5 2.11 21.64v40.42H516.3V76.17c0-7-.34-11.54-1-13.77a10.81 10.81 0 0 0-3.69-5.47 9.18 9.18 0 0 0-5.86-2.14q-6.35 0-13.64 6a48.3 48.3 0 0 0-12 15.1v42.17z"
              /><circle
                cx="60.36"
                cy="60.36"
                r="60.36"
                fill="url(#a)"
              /><path
                d="M101.15 56.88C80.79 21.38 64.69 18.46 52.94 24c-5.74 2.71-3.34 5.2-11.52 3.41-7.28-1.59-10.67-2.13-17.07.85s-9 6.83-9 8.54 1.71-2.56 6.4-3 11.1 0 16.22 3.84 5.54 5.12 5.54 6.83-6.68-.76-13.22.85c-5.78 1.42-10.24 3.41-10.67 5.12s11.63.44 16.64.43c2.38.08 4.34-.67 6 2.56 1.72 3.4 2.13 6 4.27 6.82s2.56-1.7 5.12 3.42 3.41 8.1.42 15.78-4.68 12.84-3.4 11.55c1-1 3.31-1.24 4.46-2.73-.32 2.74 0 7.78 3.65 13.4 6.4 9.81 15.76 9 29 12.39 20.61 5.19 30.87 5.49 35.19 12.53.85 1.39 1.39 2.61.48-.72-4.24-15.51-7.81-47.22-20.3-68.99z"
                fill="url(#b)"
              /><circle
                cx="55.37"
                cy="31.32"
                r="2.43"
                fill="#fff"
              /></g></g></svg>
            </div>
            <nav
              class="mt-4 space-y-8 flex-1"
              aria-label="Sidebar"
            >
              <div class="px-2 space-y-0">
                <!-- Current: "bg-gray-200 text-gray-900", Default: "text-gray-600 hover:bg-gray-50 hover:text-gray-900" -->
                <a
                  href="#"
                  class="bg-gray-200 text-gray-900 group flex items-center px-2 py-2 text-md font-medium rounded-md"
                >
                  <!-- Current: "text-gray-500", Default: "text-gray-400 group-hover:text-gray-500" -->
                  <!-- Heroicon name: outline/home -->
                  <svg
                    class="text-gray-500 mr-3 h-6 w-6"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M4 6h16M4 10h16M4 14h16M4 18h16"
                    />
                  </svg>
                  All
                </a>

                <a
                  href="#"
                  class="text-gray-600 hover:bg-gray-50 hover:text-gray-900 group flex items-center px-2 py-2 text-md font-medium rounded-md"
                >
                  <!-- Heroicon name: outline/calendar -->
                  <svg
                    class="text-gray-400 group-hover:text-gray-500 mr-3 h-6 w-6"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"
                    />
                  </svg>
                  Favourites
                </a>

                <a
                  href="#"
                  class="text-gray-600 hover:bg-gray-50 hover:text-gray-900 group flex items-center px-2 py-2 text-md font-medium rounded-md"
                >
                  <span class="inline-block relative">
                    <svg
                      class="text-gray-500 mr-3 h-6 w-6"
                      xmlns="http://www.w3.org/2000/svg"
                      fill="none"
                      viewBox="0 0 24 24"
                      stroke="currentColor"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M4 6h16M4 10h16M4 14h16M4 18h16"
                      />
                    </svg>
                    <span class="absolute top-1 right-4 block h-2 w-2 transform -translate-y-1/2 translate-x-1/5 rounded-full ring-2 ring-white bg-red-400" />
                  </span>
                  Unread
                </a>

                <a
                  href="#"
                  class="text-gray-600 hover:bg-gray-50 hover:text-gray-900 group flex items-center px-2 py-2 text-md font-medium rounded-md"
                >
                  <!-- Heroicon name: outline/search-circle -->
                  <svg
                    class="text-gray-400 group-hover:text-gray-500 mr-3 h-6 w-6"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                    aria-hidden="true"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M8 16l2.879-2.879m0 0a3 3 0 104.243-4.242 3 3 0 00-4.243 4.242zM21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                    />
                  </svg>
                  Recently Read
                </a>

                <a
                  href="#"
                  class="text-gray-600 hover:bg-gray-50 hover:text-gray-900 group flex items-center px-2 py-2 text-md font-medium rounded-md"
                >
                  <!-- Heroicon name: outline/speakerphone -->
                  <svg
                    class="text-gray-400 group-hover:text-gray-500 mr-3 h-6 w-6"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"
                    />
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                    />
                  </svg>
                  Recently Played
                </a>
              </div>
              <div class="space-y-1">
                <h3
                  id="projects-headline"
                  class="px-3 text-xs font-semibold text-gray-500 uppercase tracking-wider"
                >
                  Subscriptions
                </h3>
                <div
                  class="space-y-0"
                  role="group"
                  aria-labelledby="projects-headline"
                >
                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Website redesign
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      GraphQL API
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Customer migration guides
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>

                  <a
                    href="#"
                    class="group flex items-center px-3 py-2 text-sm font-medium text-gray-600 rounded-md hover:text-gray-900 hover:bg-gray-50"
                  >
                    <img
                      class="h-4 mr-2"
                      src="https://unavatar.now.sh/vox.com"
                      alt="Leave Me Alone Icon"
                    >
                    <span class="truncate">
                      Profit sharing program
                    </span>
                    <span class="bg-gray-100 group-hover:bg-gray-200 ml-auto inline-block py-0.5 px-3 text-xs font-medium rounded-full">
                      4
                    </span>
                  </a>
                </div>
              </div>
            </nav>
          </div>
          <div class="flex-shrink-0 flex border-t border-gray-200 p-4">
            <a
              href="#"
              class="flex-shrink-0 w-full group block"
            >
              <div class="flex items-center">
                <div>
                  <img
                    class="inline-block h-9 w-9 rounded-full"
                    src="https://images.unsplash.com/photo-1517365830460-955ce3ccd263?ixlib=rb-=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=8&w=256&h=256&q=80"
                    alt=""
                  >
                </div>
                <div class="ml-3">
                  <p class="text-sm font-medium text-gray-700 group-hover:text-gray-900">
                    Whitney Francis
                  </p>
                  <p class="text-xs font-medium text-gray-500 group-hover:text-gray-700">
                    View profile
                  </p>
                </div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="flex flex-col min-w-0 flex-1 overflow-hidden">
      <div class="flex-1 relative z-0 flex overflow-hidden">
        <main
          class="flex-1 relative z-0 overflow-y-auto focus:outline-none xl:order-last"
          tabindex="0"
        >
          <!-- Start main area-->
          <div class="absolute inset-0 py-6 px-4 sm:px-6 lg:px-8">
            <div class="h-full border-2 border-gray-200 border-dashed rounded-lg" />
          </div>
        <!-- End main area -->
        </main>
        <aside class="hidden relative xl:order-first xl:flex xl:flex-col flex-shrink-0 w-96 border-r border-gray-200">
          <!-- Start secondary column (hidden on smaller screens) -->
          <div class="absolute inset-0 py-6 px-4 sm:px-6 lg:px-8">
            <div class="h-full border-2 border-gray-200 border-dashed rounded-lg" />
          </div>
        <!-- End secondary column -->
        </aside>
      </div>
    </div>
  </div>
</template>
