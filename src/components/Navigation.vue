<template>
	<nav>
		<ul class="menu">
			<li class="menu-text"
				v-for="(link, index) in navLinks"
				:key="index"
			>
				<router-link class="link"
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

.menu-text{
  margin-top:15px;
  font-size: 18px;
  color: white;
  font-weight: bold;
  cursor: pointer;
  padding: 10px;
  border-bottom: 2px solid #080808;
  width: fit-content;
  list-style-type: none;
  
}

.menu-text:hover {
  border-bottom: 2px solid white;
}


.link {
  color: white;
  text-decoration: none;  

}

</style>