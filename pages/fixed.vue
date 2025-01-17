<template>
  <div>
    <h4>This works in dev and prod again. Both client and fallback children are elements.</h4>
    <h4>Change the fallback parent element tag to be different than the client parent element tag in ClientOnly:</h4>
    <ClientOnly>
      <div>
        <div>client</div>
      </div>

      <template #fallback>
        <!-- changed tag -->
        <span>
          <div>fallback</div>
        </span>
      </template>
    </ClientOnly>

    <h4>Change the client parent element tag to be different than the fallback parent element tag in ClientOnly:</h4>
    <ClientOnly>
      <!-- changed tag -->
      <span>
        <div>client</div>
      </span>

      <template #fallback>
        <div>
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
