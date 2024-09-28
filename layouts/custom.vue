<template>
	<Html>
			<!-- Head -->
			<Head>
					<Title>Gyan Geta Nusantara - Inovasi Kecantikan</Title>
					<Meta name="description" :content="`Gyan Geta Nusantara - Inovasi Kecantikan`" />
					<!-- <Link rel="preload" href="/test.txt" as="script" /> -->
					<!-- <Style type="text/css" :children="styleString" /> -->
			</Head>

			<!-- Header -->
			<nav-header />

			<!-- Content -->
			<slot />

			<!-- Footer -->
			<!-- <the-footer /> -->
	</Html>
</template>

<script>
definePageMeta({
  layout: "custom",
});

import NavHeader from '@/layouts/partials/NavHeader.vue'
import TheFooter from '@/layouts/partials/TheFooter.vue'

export default {
	components: {
		NavHeader,
		TheFooter,
	},
	setup() {
		return {
		}
	},
}
</script>

