<template>
  <!-- flex justify-start content-center -->
  
  <div class="h-screen w-screen">
    <div class="h-full flex justify-center items-center">
      <div class="border-teal w-108 p-8 border-t-12 bg-white mb-6 mx-12 rounded-lg shadow-lg">
        <div class="">
          <img class="block h-16 px-6 py-1 mx-auto" src="../assets/mng-logo-1.png" alt="">
        </div>
        <div class="">
          <p class="text-grey-light font-medium font-md pt-4 pb-2 text-lg">
            Welcome Back
          </p>
        </div>
        <div class="mb-4">
            <input type="text" class="block appearance-none w-full bg-white border border-grey-light hover:border-grey px-2 py-2 rounded shadow" placeholder="Email">
        </div>
        <div class="mb-4">
            <input type="password" class="block appearance-none w-full bg-white border border-grey-light hover:border-grey px-2 py-2 rounded shadow" placeholder="Password">
        </div>

        <div class="">
          <div class="py-2">
            <router-link 
              exact-active-class="navbar-item-selected" 
              tag="a"
              to="/reports"
              class="no-underline"
              href="#">
            <button class="block w-full mx-auto bg-blue-dark hover:bg-blue-light text-white font-bold py-3 px-4 rounded">
                Sign In
            </button>
          </router-link>
            
          </div>
          <div class="justify-start">
            <a class="no-underline inline-block align-baseline font-medium text-sm text-blue hover:text-blue-dark pt-2" href="#">
              Forgot your password?
            </a>
          </div>
          <div class="justify-start">
            <a class="no-underline inline-block align-baseline font-medium text-sm text-blue hover:text-blue-dark pt-2" href="#">
              Not registered? Request access now.
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "logincard"
}
</script>