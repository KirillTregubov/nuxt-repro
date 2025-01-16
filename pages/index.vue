<template>
  <div>
    <ClientOnly>
      <div>
        <div>client</div>
      </div>

      <template #fallback>
        <div>
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
