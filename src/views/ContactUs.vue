<template>
  <div class="font-sans antialiased">
    <navbar></navbar>
    <div class="flex flex-wrap">
      <div class="w-1/2 py-4  px-2">
        <p class="text-lg font-semibold">Check out our FAQ</p>
      </div>
      <div class="w-1/2 py-4  px-2">
        <p class="text-lg font-semibold">Contact Us</p>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import FilterSearch from "@/components/FilterSearch";

export default {
    name: "reports",
    components: {
      Navbar,
      FilterSearch
    }
}
</script>

<style>

</style>
