<template>
	<nav>

		<ul class="menu">
      <div class="campinglogo">
       <img src="../assets/svg/campingwhite.svg" alt="Logo" height="80" width="80" >
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
  padding-bottom: 1px;

}

.campinglogo{

  margin-top:10px;


}

.menu-text{
  margin-top:10px;
  margin-bottom:10px;
  font-size: 16px;
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