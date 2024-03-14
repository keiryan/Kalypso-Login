<template>
  <div
    class="flex-1 flex flex-col justify-between items-center overflow-scroll"
  >
    <!-- Login Container -->
    <div>
      <img class="w-48 m-8" src="../../public/images/Keiryan.png"
      alt="login-rounded-right--v1"
    </div>
    <div class="">
      <h1 class="text-xl font-bold mb-4">Register</h1>
      <div class="flex gap-4">
        <Input type="text" label="First Name" placeholder="Your first name" />
        <Input type="text" label="Last Name" placeholder="Your last name" />
      </div>

      <Input
        class="block"
        type="email"
        label="Email Address"
        placeholder="Your email"
      />

      <div class="w-full">
        <Input type="password" label="Password" placeholder="Your password" />
      </div>

      <div class="flex items-center text-sm gap-2 my-4 font-light">
        <Toggle />
        <div>
          I accept the&nbsp;<a href="#" class="text-[#5DA2E2] hover:underline"
            >Terms of Service</a
          >&nbsp;as well as&nbsp;<a
            href="#"
            class="text-[#5DA2E2] hover:underline"
            >Privacy Policy</a
          >.
        </div>
      </div>

      <div>
        <button
          class="bg-blue-500 text-white px-4 py-2 rounded-md text-sm flex gap-2 items-center my-6 mb-10 shadow-[0_1px_2px_0px_rgba(0,0,0,0.15)]"
        >
          <img
            width="24"
            height="24"
            src="https://img.icons8.com/ios/50/FFFFFF/login-rounded-right--v1.png"
            alt="login-rounded-right--v1"
          />
          Create Account
        </button>
      </div>
      <hr class="" />
      <div class="text-[#AFB4B9] text-sm text-center mt-8 font-light">
        Already have an account?
        <a href="#" class="text-[#258BE6] hover:underline font-semibold"
          >Login now.</a
        >
      </div>
    </div>
    <footer class="w-full p-8 text-[#7D8597] text-xs flex flex-col">
      <ul class="flex md:gap-8 font-light pl-0 list-none justify-center gap-4">
        <li class="hover:underline p-4">
          <a href="#">Help</a>
        </li>
        <li class="hover:underline p-4">
          <a href="#">Legal</a>
        </li>
        <li class="hover:underline p-4">
          <a href="#">Privacy</a>
        </li>
        <li class="hover:underline p-4">
          <a href="#">TOS</a>
        </li>
      </ul>
      <div class="mt-4">
        <p class="text-center font-light">&copy; Cloudklabauter</p>
      </div>
    </footer>
  </div>
</template>

<script>
import Input from "./Input.vue";
import Toggle from "./Toggle.vue";

export default {
  name: "Login",
  components: {
    Input,
    Toggle,
  },
};
</script>

<style scoped></style>
