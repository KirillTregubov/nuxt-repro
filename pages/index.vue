<template>
  <div>
    <h4>This works in dev and prod.</h4>
    <h4>Fallback child is textContent in ClientOnly:</h4>
    <ClientOnly>
      <div>
        <div>client</div>
      </div>

      <template #fallback>
        <div>
          fallback
        </div>
      </template>
    </ClientOnly>

    <h4>Client child is textContent in ClientOnly:</h4>
    <ClientOnly>
      <div>
        client
      </div>

      <template #fallback>
        <div>
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
