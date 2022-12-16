<template>
  <div>
    <NuxtWelcome />
  </div>
</template>
<script setup>

const error = new Error('new Error')
throw createError({
		stack: error.stack,
		statusCode: 404,
		statusMessage: 'Page Not Found',
		message: 'Page Not Found',
		data: error.message,
		fatal: true,
	})
</script>