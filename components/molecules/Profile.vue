<template>
	<div class="flex items-center">
		<img src="https://github.com/Alexssmusica.png" alt="Alex Santos" class="mr-6 w-20 h20 rounded-full">
		<div class="flex flex-col w-full">
			<strong class="text-title text-2xl">Alex Santos</strong>
			<p class="flex items-center">
				<img src="icons/level.svg" alt="level" class="mr-2">
				<span class="text-base">Level {{ level }}</span>
			</p>
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import { mapState } from 'vuex';

export default Vue.extend({
	computed: mapState('Challenges', ['level'])
});
</script>
