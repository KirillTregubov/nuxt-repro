<template>
  <div>
    <nav>
      <NuxtLink to="/">One child</NuxtLink>
      <NuxtLink to="/broken">Two fallback children (broken)</NuxtLink>
      <NuxtLink to="/also-broken">Two client children (broken)</NuxtLink>
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
