<template>
	<div class="bg-home mb-5" style="height:100vh">
		<div class="container-fluid mb-5">
			<b-row>
				<b-col md="4">
					<h3 class="text-white my-4">Portfolio</h3>
				</b-col>

				<b-col md="8">
					<div class="d-flex justify-content-center align-items-center my-4">
						<b-link class="text-dark mx-3">About Me</b-link>
						<b-link class="text-dark mx-3">Portfolio</b-link>
						<b-btn pill class="mx-3 px-5" variant="primary">Download CV</b-btn>
					</div>
				</b-col>
			</b-row>
		</div>

		<div class="container">
			<b-row class="justify-content-center">
				<b-col md="12">
					<div class="d-flex align-items-center">
						<div>
							<b-img class="mb-5" width="450" height="450" :src="require('../assets/photo.png')" />
						</div>
						<div class="pl-5">
							<div class="font-weight-bold" style="font-size:60px">MY <span class="text-primary">WORK</span></div>
							<h4>Web & Visual Designer</h4>
						</div>
					</div>
				</b-col>
			</b-row>
		</div>
	</div>
</template>

<script>
export default {
	name: 'Hello'
}
</script>

<style scoped>
	.bg-home {
		background-image: url('../assets/Group12.png');
		background-repeat: no-repeat;
  	background-attachment: fixed;
	}
</style>