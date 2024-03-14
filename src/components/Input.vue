<template>
  <div class="w-full py-4 text-sm flex flex-col">
    <label class="pb-1 font-light">{{ label }}</label>
    <input
      :type="type"
      class="border border-gray-200 p-2 w-full transparent bg-white rounded-[4px] focus:outline-none shadow-[0_1px_1px_0px_rgba(0,0,0,0.13)] capitalize"
      :placeholder="placeholder"
    />
  </div>
</template>

<script>
export default {
  name: "Input",
  props: {
    type: {
      type: String,
      default: "text",
    },
    placeholder: {
      type: String,
      default: "",
    },
    label: {
      type: String,
      default: "",
    },
  },
};
</script>

<style></style>
