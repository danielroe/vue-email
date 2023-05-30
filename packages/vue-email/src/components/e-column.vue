<template>
  <td v-bind="$props" data-id="__vue-email-column" :style="style" role="presentation">
    <slot />
  </td>
</template>

<script lang="ts" setup>
import type { HTMLAttributes } from 'vue';

interface Props extends /* @vue-ignore */ Omit<HTMLAttributes, 'style'> {
  style?: string | object;
}

defineProps<Props>();
</script>
