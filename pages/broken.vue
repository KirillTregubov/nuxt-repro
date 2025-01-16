<template>
  <div>
    <ClientOnly>
      <div>
        <div>client</div>
      </div>

      <template #fallback>
        <div>
          <div>
            fallback
            <!-- NOTE: can also add here to break -->
          </div>
          <!-- NOTE: added second child -->
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
