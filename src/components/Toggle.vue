<template>
  <!-- Container -->
  <div
    class="w-10 h-6 rounded-full relative transition-all duration-300 ease-in-out hover:cursor-pointer"
    @click="toggle"
    :class="!isActive ? 'bg-[#C3C3C3]' : 'bg-[#258BE6]'"
  >
    <!-- Inner Circle -->
    <div
      class="w-5 h-5 bg-white absolute top-0.5 rounded-full transition-all duration-300 ease-in-out shadow-[0_4px_4px_0px_rgba(0,0,0,0.3)]"
      :class="isActive ? 'toggle-active' : 'toggle-inactive'"
    />
  </div>
</template>

<script>
export default {
  name: "Toggle",
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    toggle() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style scoped>
.toggle-active {
  left: calc(100% - 1.25rem - 2px);
}

.toggle-inactive {
  left: 2px;
}

.inner-toggle {

}
</style>
