<template>
  <div>
    <UiNavbar>
      <UiContainer class="flex h-14 items-center justify-between">
        <p class="font-semibold">UI Thing</p>
        <nav class="hidden items-center gap-5 sm:flex">
          <NuxtLink
            class="text-sm text-muted-foreground transition-colors hover:text-foreground"
            v-for="l in ['Home', 'About', 'Contact', 'Projects']"
            :key="l"
            to="/"
            >{{ l }}</NuxtLink
          >
        </nav>
      </UiContainer>
    </UiNavbar>
  </div>
</template>
