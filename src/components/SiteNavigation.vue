<template>
    <header class="bg-at-green text-white">
    <nav class="container py-2 px-4 flex flex-col gap-4 items-center sm:flex-row">
      <div class="flex items-center gap-x-4">
        <img class="w-14" src="../assets/images/dumbbell-light.png" alt="" />
        <h1 class="text-lg">Workout Tracker</h1>
      </div>
      <ul class="flex flex-1 justify-end gap-x-10">
        <router-link class="cursor-pointer" :to="{name: 'home'}">Home</router-link>
        <router-link class="cursor-pointer" :to="{name: 'Create'}">Create</router-link>
        <router-link class="cursor-pointer" :to="{name: 'Login'}">Login</router-link>
        <router-link class="cursor-pointer" :to="{name: 'Register'}">Register</router-link>
        <li class="cursor-pointer">Logout</li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {

}
</script>

<style>

</style>