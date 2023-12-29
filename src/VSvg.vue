<script setup lang="ts">
const props = withDefaults(
  defineProps<{
    name: string
    // NOTE: 複数の色を受け取りたい SVG が必要なら再度検討
    color?: string
  }>(),
  {
    color: () => "",
  },
)

const componentName = computed(() => `svg-${props.name}`)
</script>

<template>
  <component :is="componentName" class="svg" />
</template>

<style scoped>
.svg {
  --color: v-bind(color);
}
</style>
