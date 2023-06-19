<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex justify-between">
        <ul class="flex gap-3">
          <li>
            <NuxtLink to="/" class="font-bold mx-30">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products" class="font-bold mx-30">Products</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/login" class="font-bold mx-30">Login</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>
    <div class="container mx-auto p-4">
      <slot></slot>
    </div>
  </div>
</template>

<style>
.router-link-active{
    color: rgb(137, 199, 140);
}
</style>
