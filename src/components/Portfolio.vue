<template>
  <div class="container mb-5">
		<b-row class="justify-content-center mb-5">
			<b-col md="3">
				<b-card class="shadow">
					<div class="p-3">
						<b-img class="mb-5" width="50" height="50" :src="require('../assets/stopwatch.png')" />
						<h5>On Time</h5>
						<p class="mb-5">All i want to have client setisfaction & this is my aim</p>
						<b-button to="/" variant="primary">Learn more</b-button>
					</div>
				</b-card>
			</b-col>

			<b-col md="3">
				<b-card class="shadow">
					<div class="p-3">
						<b-img class="mb-5" width="50" height="50" :src="require('../assets/safe-box.png')" />
						<h5>Clean Work</h5>
						<p class="mb-5">All i want to have client setisfaction & this is my aim</p>
						<b-button to="/" variant="primary">Learn more</b-button>
					</div>
				</b-card>
			</b-col>
			<b-col md="3">
				<b-card class="shadow">
					<div class="p-3">
						<b-img class="mb-5" width="50" height="50" :src="require('../assets/icon.png')" />
						<h5>Client Setisfaction</h5>
						<p class="mb-5">All i want to have client setisfaction & this is my aim</p>
						<b-button to="/" variant="primary">Learn more</b-button>
					</div>
				</b-card>
			</b-col>
		</b-row>

		<div class="text-center">
			<h2>My Porfolio</h2>
			<p class="text-secondary">Web & APP</p>
		</div>
		<b-row class="justify-content-center">
			<b-col md="4">
				<b-img width="372" height="372" :src="require('../assets/1.png')" />
			</b-col>
			<b-col md="4">
				<b-img width="372" height="372" :src="require('../assets/2.png')" />
			</b-col>
			<b-col md="4">
				<b-img width="372" height="372" :src="require('../assets/3.png')" />
			</b-col>
			<b-col md="8" class="mt-2">
				<b-img width="751" height="372" :src="require('../assets/4.png')" />
			</b-col>
			<b-col md="4" class="mt-2">
				<b-img width="372" height="372" :src="require('../assets/5.png')" />
			</b-col>
			<b-col md="4" class="mt-2">
				<b-img width="372" height="372" :src="require('../assets/6.png')" />
			</b-col>
			<b-col md="4" class="mt-2">
				<b-img width="372" height="372" :src="require('../assets/7.png')" />
			</b-col>
			<b-col md="4" class="mt-2">
				<b-img width="372" height="372" :src="require('../assets/8.png')" />
			</b-col>
		</b-row>

  </div>
</template>

<script>
export default {
  name: 'Porfolio'
}
</script>

<style>

</style>