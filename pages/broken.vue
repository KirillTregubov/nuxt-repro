<template>
  <div>
    <h4>This works in dev, and when loaded through the client in prod. Does NOT work on fresh prod load (reload the page to see).</h4>
    <h4>Both fallback and client children are elements in ClientOnly:</h4>
    <ClientOnly>
      <div>
        <div>client</div>
      </div>

      <template #fallback>
        <div>
          <!-- NOTE: turned textContent into child -->
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
