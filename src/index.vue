<template>
  <component
    :is="prefix ? `${prefix}-${type}` : `${field.type}`"
    v-bind="$props"
  />
</template>

<script>
export default {
  name: "sniffer",
  props: {
    prefix: {
      type: [String],
      default: ""
    },
    type: {
      type: [String],
      default: ""
    }
  }
};
</script>
