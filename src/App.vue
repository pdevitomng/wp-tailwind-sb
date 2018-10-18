<template>
  <div id="app" class="min-h-screen bg-white font-sans antialiased border-t-4 border-blue">
    <div class="hidden sm:block bg-white border-b select-none">
        <div class="px-4 flex items-end justify-between text-md">
          <div class="px-4 flex items-end" role="left">
            <div>
              <img class="block h-16 px-6 py-1" src="@/assets/mng-logo-1.png" alt="">
            </div>

            <div class="flex -mb-px mr-6">
              <a class="no-underline text-grey-dark flex item-center pt-6 pb-2 border-b border-transparent hover:text-blue-light hover:border-blue-light" href="#">
                <svg class="fill-current inline-block h-4 w-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M14 5h2v14H4V5h2V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v1zm3 0h1a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-1V5zM3 5v14H2a2 2 0 0 1-2-2V7c0-1.1.9-2 2-2h1zm5-1v1h4V4H8z"/></svg>
                Orders
              </a>
            </div>

            <div class="flex -mb-px mr-6">
              <a class="no-underline text-blue-dark font-medium flex item-center pt-6 pb-2 border-b-2 border-blue-dark" href="#">
                <!-- 
                1) https://github.com/dukestreetstudio/zondicons/tree/master/src
                2) click on one and select 'raw'
              -->
                <svg class="fill-current inline-block h-4 w-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M6 4H5a1 1 0 1 1 0-2h11V1a1 1 0 0 0-1-1H4a2 2 0 0 0-2 2v16c0 1.1.9 2 2 2h12a2 2 0 0 0 2-2V5a1 1 0 0 0-1-1h-7v8l-2-2-2 2V4z"/></svg>
                Reports
              </a>
            </div>

            <div class="flex -mb-px mr-6">
              <a class="no-underline text-grey-dark flex item-center pt-6 pb-2 border-b border-transparent hover:text-blue-light hover:border-blue-light" href="#">
                <!-- <svg class="fill-current inline-block h-4 w-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M19 11a7.5 7.5 0 0 1-3.5 5.94L10 20l-5.5-3.06A7.5 7.5 0 0 1 1 11V3c3.38 0 6.5-1.12 9-3 2.5 1.89 5.62 3 9 3v8zm-9 1.08l2.92 2.04-1.03-3.41 2.84-2.15-3.56-.08L10 5.12 8.83 8.48l-3.56.08L8.1 10.7l-1.03 3.4L10 12.09z"/></svg> -->
                <svg class="fill-current inline-block h-4 w-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M7 8a4 4 0 1 1 0-8 4 4 0 0 1 0 8zm0 1c2.15 0 4.2.4 6.1 1.09L12 16h-1.25L10 20H4l-.75-4H2L.9 10.09A17.93 17.93 0 0 1 7 9zm8.31.17c1.32.18 2.59.48 3.8.92L18 16h-1.25L16 20h-3.96l.37-2h1.25l1.65-8.83zM13 0a4 4 0 1 1-1.33 7.76 5.96 5.96 0 0 0 0-7.52C12.1.1 12.53 0 13 0z"/></svg>
                Administration
              </a>
            </div>
          </div>
          <div class="px-4 flex items-end" role="right">
            <div class="flex -mb-px mr-6">
              <a class="no-underline text-grey-dark flex item-center pt-6 pb-2 border-b border-transparent hover:text-blue-light hover:border-blue-light" href="#">
                <svg class="fill-current inline-block h-4 w-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M10 20a10 10 0 1 1 0-20 10 10 0 0 1 0 20zm2-13c0 .28-.21.8-.42 1L10 9.58c-.57.58-1 1.6-1 2.42v1h2v-1c0-.29.21-.8.42-1L13 9.42c.57-.58 1-1.6 1-2.42a4 4 0 1 0-8 0h2a2 2 0 1 1 4 0zm-3 8v2h2v-2H9z"/></svg>
                Contact Us
                </a>
            </div>

            <div class="flex -mb-px mr-6">
              <a class="no-underline text-grey-dark flex item-center pt-6 pb-2 border-b border-transparent hover:text-blue-light hover:border-blue-light" href="#">
                <svg class="fill-current inline-block h-4 w-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M10 20a10 10 0 1 1 0-20 10 10 0 0 1 0 20zM7 6v2a3 3 0 1 0 6 0V6a3 3 0 1 0-6 0zm-3.65 8.44a8 8 0 0 0 13.3 0 15.94 15.94 0 0 0-13.3 0z"/></svg>
                My Account
                </a>
            </div>

            <div class="flex -mb-px mr-6">
              <a class="no-underline text-grey-dark flex item-center pt-6 pb-2 border-b border-transparent hover:text-blue-light hover:border-blue-light" href="#">
                Sign Out
                <!-- notepad: https://material.io/tools/icons/?icon=launch&style=baseline -->
                <svg class="fill-current inline-block h-4 w-4 ml-2" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M0 0h24v24H0z" fill="none"/><path d="M19 19H5V5h7V3H5c-1.11 0-2 .9-2 2v14c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2v-7h-2v7zM14 3v2h3.59l-9.83 9.83 1.41 1.41L19 6.41V10h2V3h-7z"/></svg>
              </a>
            </div>
          </div>
        </div>
      </div>

    <div role="filter-row" class="flex uppercase text-2xl select-none ml-16 pt-12">
      <div class="mx-4 font-medium border-b-2 border-green">All</div>
      <div class="mx-4 hover:cursor-pointer hover:opacity-50">On Hold</div>
      <div class="mx-4 hover:cursor-pointer hover:opacity-50">In The Lab</div>
      <div class="mx-4 hover:cursor-pointer hover:opacity-50">Complete</div>
      <div class="mx-4 hover:cursor-pointer hover:opacity-50">Rejected/Cancelled</div>
    </div>

    <div role="search-bar" class="flex items-center pt-12 px-6">
      <div class="ml-8 p-2">
        <svg class="fill-current inline-block h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.9 14.32a8 8 0 1 1 1.41-1.41l5.35 5.33-1.42 1.42-5.33-5.34zM8 14A6 6 0 1 0 8 2a6 6 0 0 0 0 12z"/></svg>
      </div>
      <!-- <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight focus:outline-none focus:shadow-outline" type="text" placeholder="Search by name, date of birth, identifier, physician, or test code"> -->
      <input class="appearance-none border-b border-grey-light w-full py-2 text-grey-darker leading-tight focus:outline-none" type="text" placeholder="Search by name, date of birth, identifier, physician, or test code">
    </div>

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
          <td class="border-t-2 px-2 text-center">
            <div class="inline-block px-6 rounded-full bg-green-light text-green-darker font-semibold py-2">
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
          <td class="border-t-2 px-2">
            <div class="inline-flex px-6 rounded-full bg-green-light text-green-darker font-semibold py-2">
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

<style>
/*
    1) NPM: npm install tailwindcss --save-dev
    2) package.json: 
      "postcss": {
          "plugins": {
            "tailwindcss": "./tailwind.js",
            "autoprefixer": {}
          }
        },
    3) VS Code Terminal: ./node_modules/.bin/tailwind init tailwind.js
    4) @tailwinds, in order, below
    5) npm run serve
   */

@tailwind preflight;
@tailwind components;
@tailwind utilities;
@import url("https://rsms.me/inter/inter-ui.css");
</style>

