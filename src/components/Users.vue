<template>
	<div class="container-fluid text-center">
		<div class="mb-5">
			<h3>Valuable Testimonial</h3>
			<p class="text-secondary">See People Say About Me</p>

			<div>
				<b-card v-for="user in users" :key="user.email">
					<div>
						{{user}}
					</div>
				</b-card>
			</div>
		</div>
		
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
			users: null,
			sliding: null,
			slide: 0
		}
	},
	mounted () {
		return axios.get('https://randomuser.me/api/')
		.then((res) => {
			this.users = res.data.results
		})
		.catch(err => {
			console.log(err)
		})
	},
	methods: {
		onSlideStart(slide) {
			this.sliding = true
		},
		onSlideEnd(slide) {
			this.sliding = false
		}
	}
}
</script>