<template>
  <div>Catch all route "{{ route.path }}"</div>
</template>

<script setup lang="ts">
const route = useRoute();
if (route.path.includes('.')) {
  throw createError({
    statusCode: 404,
    statusMessage: 'Not found',
    fatal: true,
  });
}
</script>
