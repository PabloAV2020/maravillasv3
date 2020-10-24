<template>
	<nav>
		<ul class="menu">
			<li
				v-for="(link, index) in navLinks"
				:key="index"
			>
				<router-link
					:to="link.path"
				>
					{{ link.text }}
				</router-link>
			</li>
		</ul>
	</nav>
</template>

<script>
export default {
	props: ['navLinks'],
}
</script>

<style scoped>

.menu {
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin-top: 10px;
  height: 60px;
}


</style>