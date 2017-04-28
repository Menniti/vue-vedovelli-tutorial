
<script>
	export default {
		methods: {
			mudarDados () {
				const payload = {
					name: 'OutroNome',
					email: 'outro@email.com',
					level: 'usuario-raso'
				}

				this.$store.commit('CHANGE_USER',
					payload)
			}
		}

	}
</script>

<template>
	<div>
		<button @click="mudarDados">Mudar dados do usuário</button>
	</div>
</template>