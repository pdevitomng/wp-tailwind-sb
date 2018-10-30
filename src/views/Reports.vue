<template>
    <div>
      <navbar></navbar>
      <div role="filter-row" class="flex flex-wrap uppercase text-2xl select-none ml-16 pt-12">
        <!-- <div :selected="true"  class="mx-4" :class="[selected ? 'font-medium border-b-2 border-green' : 'hover:cursor-pointer hover:opacity-50']">All</div>
        <div :selected="false" class="mx-4" :class="[selected ? 'font-medium border-b-2 border-green' : 'hover:cursor-pointer hover:opacity-50']">On Hold</div>
        <div :selected="false" class="mx-4" :class="[selected ? 'font-medium border-b-2 border-green' : 'hover:cursor-pointer hover:opacity-50']">In The Lab</div>
        <div :selected="false" class="mx-4" :class="[selected ? 'font-medium border-b-2 border-green' : 'hover:cursor-pointer hover:opacity-50']">Complete</div>
        <div :selected="false" class="mx-4" :class="[selected ? 'font-medium border-b-2 border-green' : 'hover:cursor-pointer hover:opacity-50']">Rejected/Cancelled</div> -->
        <div v-for="status in StatusOptions" :key=status.index  class="mx-4" :class="[status.name == selectedStatus ? 'font-medium border-b-2 border-green' : 'hover:cursor-pointer hover:opacity-50']" @click= "selectedStatus=status.name">{{status.name}}</div>
        <!-- <div 
          v-for="status in StatusOptions" 
          :key=status.index 
          class="mx-4" 
          @click= "selectedStatus=status.name">
            {{status.name}}
        </div> -->
      </div>

      <div role="search-bar" class="flex items-center pt-12 px-6">
      <div class="ml-8 p-2">
          <svg class="fill-current inline-block h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.9 14.32a8 8 0 1 1 1.41-1.41l5.35 5.33-1.42 1.42-5.33-5.34zM8 14A6 6 0 1 0 8 2a6 6 0 0 0 0 12z"/></svg>
      </div>
      <!-- <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" type="text" placeholder="Search by name, date of birth, identifier, physician, or test code"> -->
      <input class="appearance-none border-b border-grey-light w-full py-2 text-grey-darker leading-tight focus:outline-none" type="text" placeholder="Search by name, date of birth, identifier, physician, or test code">
      </div>

      <div class="py-6 px-4 font-bold">This will be the filter val: {{selectedStatus}}</div>

      <div role="table" class = "container mx-auto py-6">
      <table class="container mx-auto border-2 rounded-lg shadow py-6">
          <tr class = "border-y-2">
          <th class="text-left uppercase bg-grey-lighter font-semibold font-grey-dark py-2">Name</th>
          <th class="text-left uppercase bg-grey-lighter font-semibold font-grey-dark py-2">Status</th>
          </tr>
          <tr class = "border-t-2 border-y-2 py-4">
          <td class="py-4 px-4">
              <div class="text-lg font-semibold pb-1">Paul DeVito</div>
              <div class="text-xs text-grey-dark">06/18/1991</div>
          </td>
          <td class="border-t-2 px-2 text-center w-1/6">
              <div class="inline-block px-4 rounded-full bg-green-light text-green-darker font-semibold text-sm py-1">
              Complete
              </div>
          </td>
          </tr>
      </table>
      </div>

      <div role="table" class = "container mx-auto py-6">
      <table class="border-2 shadow py-6">
          <tr class = "border-y-2">
          <th class="text-left uppercase bg-grey-lighter font-semibold font-grey-dark py-2 px-2">Name</th>
          <th class="text-left uppercase bg-grey-lighter font-semibold font-grey-dark py-2 px-2">DOB</th>
          <th class="text-left uppercase bg-grey-lighter font-semibold font-grey-dark py-2 px-2">Status</th>
          </tr>
          <tr class = "border-t-2 border-y-2 py-4">
          <td class="py-4 px-4">
              <div class="">Paul DeVito</div>
          </td>
          <td>
              <div class="">06/18/1991</div>
          </td>
          <td class="border-t-2 px-2  w-1/6">
              <div class="inline-flex px-4 rounded-full bg-green-light text-green-darker font-semibold text-sm py-1">
              Complete
              </div>
          </td>
          </tr>
      </table>
      </div>
      <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
      </div>
      <router-view/> -->
    </div>
</template>

<script>
import Navbar from "@/components/Navbar";

export default {
    name: "reports",
    components: {
      Navbar
    },
    data() {
    return {
        selectedStatus: "ALL",
        StatusOptions: [
          {id: 1, name: 'ALL', selected: true},
          {id: 2, name: 'ON HOLD', selected: false},
          {id: 3, name: 'IN THE LAB', selected: false},
          {id: 4, name: 'COMPLETE', selected: false},
          {id: 5, name: 'REJECTED/CANCELLED', selected: false}
        ]
    }
  },
}
</script>
