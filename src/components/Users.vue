<template>
	<div class="container-fluid text-center">
		<div class="mb-5">
			<h3>Valuable Testimonial</h3>
			<p class="text-secondary">See People Say About Me</p>
		</div>

		<b-row class="justify-content-center mb-5">
			<b-col md="5">
				<b-card class="shadow-lg">
					<div class="mb-5">
						<b-img :src="user.picture.medium"></b-img>
					</div>
					<div>
						<h5>{{user.name.first}} {{user.name.last}},{{user.location.city}}</h5>
					</div>
				</b-card>
			</b-col>
		</b-row>
		
		<div class="mb-5">
			<div>
				<h3>Want To Hire Me?</h3>
				<p class="text-secondary">If You Like My Work</p>
			</div>

			<b-row class="justify-content-center">
				<b-col md="4">
					<b-input-group>
						<b-form-input placeholder="enter your email"></b-form-input>
						<b-input-group-append>
							<b-button variant="outline-primary">Hire Me</b-button>
						</b-input-group-append>
					</b-input-group>
				</b-col>
			</b-row>
		</div>
	</div>
</template>

<script>
import axios from 'axios'

export default {
	name: 'User',
	data() {
		return {
			user: null,
		}
	},
	mounted () {
		return axios.get('https://randomuser.me/api/')
		.then((res) => {
			this.user = res.data.results[0]
		})
		.catch(err => {
			console.log(err)
		})
	}
}
</script>