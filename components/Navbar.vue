<template>
  <div>
    <UiNavbar>
      <UiContainer class="flex h-14 items-center justify-between">
        <div class="flex flex-row gap-4">
          <!-- TODO: add logo using NuxtImage -->
          <p>Logo</p>
          <p class="font-semibold">Aggie Coding Club</p>
        </div>
        <nav class="hidden items-center gap-5 sm:flex">
          <NuxtLink
            class="text-sm uppercase text-muted-foreground transition-colors hover:text-foreground"
            v-for="l in ['About', 'Schedule', 'Officers', 'Sponsors']"
            :key="l"
            to="/"
            >{{ l }}
          </NuxtLink>
        </nav>
      </UiContainer>
    </UiNavbar>
  </div>
</template>
