<template>
	<NuxtLayout>
		<div class="error-page">
			{{error.message}}
		</div>
	</NuxtLayout>
</template>

<script setup lang="ts">
	import { NuxtError } from '#app'
	import { PropType } from 'vue'

	const props = defineProps({
		error: Object as PropType<NuxtError>,
	})

</script>
