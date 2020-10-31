<template>
	<nav>

		<ul class="menu">
      <div class="campinglogo">
       <img src="/Users/pabloav/VueSites/website-v3/src/assets/svg/campingwhite.svg" alt="Logo" >
      </div>
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
  background:#1a4221;
  padding-bottom: 15px;

}

.menu-text{
  margin-top:15px;
  margin-bottom:15;
  font-size: 18px;
  color: white;
  font-weight: bold;
  cursor: pointer;
  padding: 10px;
  width: fit-content;
  list-style-type: none;
  
}

.link {
  color: white;
  text-decoration: none;  
  border-bottom: 2px solid black;
  padding:10px;  

}

.link:hover {
border-bottom: 2px solid white;

}

.router-link-exact-active {
 
  border-bottom: 2px solid white;


} 


</style>