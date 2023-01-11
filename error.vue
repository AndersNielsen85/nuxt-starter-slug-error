
<template>
<div>error page</div>
</template>

<script setup lang="ts">
const props = defineProps({
  error: Object,
})

const handleError = () => clearError({ redirect: '/' });
</script>