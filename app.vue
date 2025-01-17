<template>
  <div>
    <nav>
      <NuxtLink to="/">One child is textContent</NuxtLink>
      <NuxtLink to="/broken">Both children are elements (broken)</NuxtLink>
      <NuxtLink to="/different-broken">Both children are elements (broken)</NuxtLink>
      <NuxtLink to="/fixed">Different parent elements (fixed)</NuxtLink>
    </nav>
    <NuxtPage />
  </div>
</template>

<style>
a {
  display: block;
}

nav {
  margin-bottom: 1rem;
}
</style>
