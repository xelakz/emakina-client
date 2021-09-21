<template>
    <div class="login mx-auto bg-gray-100 mt-40 rounded-lg">
      <div class="p-8">
        <div class="flex justify-center">
            <div class="text-3xl font-bold">Emakina Client Login</div>
        </div>
        <form class="mt-8 space-y-6" action="#" method="POST">
            <input type="hidden" name="remember" value="true">
            <div class="rounded-md shadow-sm -space-y-px">
                <div>
                <label for="email-address" class="sr-only">Email address</label>
                <input id="email-address" name="email" type="email" autocomplete="email" required
                class="appearance-none rounded-none relative block w-full px-3 py-2 border
                border-gray-300 placeholder-gray-500 text-gray-900 rounded-t-md
                focus:outline-none focus:ring-indigo-500
                focus:border-indigo-500 focus:z-10 sm:text-sm" placeholder="Email address">
                </div>
                <div>
                <label for="password" class="sr-only">Password</label>
                <input id="password" name="password" type="password" autocomplete="current-password"
                required class="appearance-none rounded-none relative block w-full px-3 py-2 border
                border-gray-300 placeholder-gray-500 text-gray-900 rounded-b-md
                focus:outline-none focus:ring-indigo-500
                focus:border-indigo-500 focus:z-10 sm:text-sm" placeholder="Password">
                </div>
            </div>

            <div class="flex items-center justify-between">
                <div class="text-sm">
                    <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500">
                        Forgot your password?
                    </a>
                </div>
                <div class="text-sm">
                  <router-link to="/register" class="font-medium text-indigo-600
                  hover:text-indigo-500">
                    Register
                  </router-link>
                </div>
            </div>

            <div>
                <button type="button" class="group relative w-full flex justify-center py-2 px-4
                border border-transparent text-sm font-medium rounded-md text-white bg-indigo-600
                hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2
                focus:ring-indigo-500">
                Sign in
                </button>
            </div>
        </form>
      </div>
    </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Login',
});
</script>
<style>
.login {
    max-width: 500px;
}

  .auth {
    width: 300px;
  }

  .auth .btn-wrapper {
    text-align: right;
  }
</style>
