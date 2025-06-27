<script setup>
import { LinktreeIcon } from 'vue3-simple-icons'

const { linktree } = useAppConfig()
</script>

<template>
  <main
    class="grid pt-8 pb-8 lg:grid-cols-2 place-items-center md:py-12"
  >
    <div>
      <h1
        class="text-3xl font-bold lg:text-5xl xl:text-6xl lg:tracking-tight xl:tracking-tighter"
      >
        link.lenzfliker.com
      </h1>
      <p class="max-w-xl mt-4 text-lg text-slate-600">
        manuja's link shortner. looking for linktree?
      </p>
      <div class="flex flex-col gap-3 mt-6 sm:flex-row">
        <HomeLink
          size="lg"
          type="outline"
          rel="noopener"
          :href="linktree"
          title="Open Linktree"
          class="flex items-center justify-center gap-1"
          target="_blank"
        >
          <LinktreeIcon
            class="w-5 h-5"
          />
          Open Linktree
        </HomeLink>
      </div>
    </div>
  </main>
</template>
