<template>
  <div>Catch all route</div>
</template>

<script setup lang="ts">
throw createError({
  statusCode: 404,
  statusMessage: 'Not found',
  fatal: true,
});
</script>
