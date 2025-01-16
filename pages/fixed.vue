<template>
  <div>
    <ClientOnly>
      <!-- changed tag -->
      <span>
        <div>client</div>
      </span>

      <template #fallback>
        <div>
          <div>fallback</div>
          <!-- NOTE: added second child -->
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
