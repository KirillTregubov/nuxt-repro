<template>
  <div>
    <h4>This is also broken ONLY on a fresh prod load (reload the page to see).</h4>
    <h4>Both fallback and client children are elements, and the client child is enclosed in a Transition element in ClientOnly:</h4>
    <ClientOnly>
      <div>
        <Transition>
          <div>client</div>
        </Transition>
      </div>

      <template #fallback>
        <div>
          <div>fallback</div>
        </div>
      </template>
    </ClientOnly>
  </div>
</template>
