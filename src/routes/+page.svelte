<script>
  let imageError = false;
</script>

<div class="flex min-h-screen flex-col items-center justify-center bg-gray-50 p-8">
  <div class="w-full max-w-md">
    <div class="mb-10 text-center">
      <div class="mx-auto mb-4 h-16 w-16 rounded-full bg-gray-900 overflow-hidden border-2 border-zinc-800">
        {#if !imageError}
          <img 
            src="https://unavatar.io/twitter/src_rip" 
            alt="Profile Avatar"
            class="h-full w-full object-cover"
            on:error={() => imageError = true}
          />
        {:else}
          <div class="h-full w-full flex items-center justify-center text-xl font-medium text-white">
            S
          </div>
        {/if}
      </div>
      <h1 class="mb-1 text-2xl font-medium text-gray-900">src.rip</h1>
      <p class="text-gray-600">Elixir / Phoenix LiveView / Svelte Developer</p>
    </div>

    <div class="space-y-4">
      <a
        href="https://github.com/srcrip"
        target="_blank"
        rel="noopener noreferrer"
        class="flex items-center rounded-xl border border-gray-200 bg-white p-4 text-gray-900 transition-all duration-200 hover:border-gray-300 hover:shadow-sm"
      >
        <svg class="mr-3 h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
          <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
        </svg>
        <span class="font-medium">GitHub</span>
      </a>

      <a
        href="https://blog.src.rip"
        target="_blank"
        rel="noopener noreferrer"
        class="flex items-center rounded-xl border border-gray-200 bg-white p-4 text-gray-900 transition-all duration-200 hover:border-gray-300 hover:shadow-sm"
      >
        <svg class="mr-3 h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
          <path d="M11.25 4.533A9.707 9.707 0 0 0 6 3a9.735 9.735 0 0 0-3.25.555.75.75 0 0 0-.5.707v14.25a.75.75 0 0 0 1 .707A8.237 8.237 0 0 1 6 18.75c1.995 0 3.823.707 5.25 1.886V4.533ZM12.75 20.636A8.214 8.214 0 0 1 18 18.75c.966 0 1.89.166 2.75.47a.75.75 0 0 0 1-.708V4.262a.75.75 0 0 0-.5-.707A9.735 9.735 0 0 0 18 3a9.707 9.707 0 0 0-5.25 1.533v16.103Z"/>
        </svg>
        <span class="font-medium">Blog</span>
      </a>

      <a
        href="https://twitter.com/src_rip"
        target="_blank"
        rel="noopener noreferrer"
        class="flex items-center rounded-xl border border-gray-200 bg-white p-4 text-gray-900 transition-all duration-200 hover:border-gray-300 hover:shadow-sm"
      >
        <svg class="mr-3 h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
          <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
        </svg>
        <span class="font-medium">Twitter</span>
      </a>
    </div>
  </div>
</div>
