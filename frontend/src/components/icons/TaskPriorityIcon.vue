<template>
  <div class="grid place-items-center">
    <div
      class="h-3 w-3 rounded-full"
      :class="{
        'bg-red-500': priority === 'High',
        'bg-yellow-500': priority === 'Medium',
        'bg-gray-300': priority === 'Low',
      }"
    ></div>
  </div>
</template>
<script>
export default {
  name: 'TaskPriorityIcon',
  props: {
    priority: {
      type: String,
      required: true,
    },
  },
}
</script>
