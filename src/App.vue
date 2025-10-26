<script setup lang="ts"></script>

<template>
  <Suspense>
    <UApp>
      <UHeader>
        <template #left>
          <RouterLink to="/">Home</RouterLink>
        </template>
        <template #right>
          <UColorModeButton />
        </template>
      </UHeader>

      <UMain>
        <RouterView />
      </UMain>

      <USeparator />

      <UFooter>
        <template #left>
          <p class="text-sm text-muted">Built with Nuxt UI • © {{ new Date().getFullYear() }}</p>
        </template>

        <template #right>
          <UButton
            to="https://github.com/nuxt-ui-templates/starter-vue"
            target="_blank"
            icon="simple-icons:github"
            aria-label="GitHub"
            color="neutral"
            variant="ghost"
          />
        </template>
      </UFooter>
    </UApp>
  </Suspense>
</template>

<style scoped></style>
