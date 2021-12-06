<template>
	<div>
		<nav>
			<ul class="topnav">
				<li><a href="">Home</a></li>
				<li><a href="">About</a></li>
				<li><a href="">Contact</a></li>
				<li><a href="">FAQ</a></li>
			</ul>
		</nav>
		<h1>hello nav</h1>
	</div>
</template>

<script>
	export default {

	}
</script>
<!-- Scoped is allow this css for only this page and block css for other component -->
<style scoped>
	ul.topnav {
		list-style-type: none;
		margin: 0;
		padding: 0;
		overflow: hidden;
		background-color: #333;
		font-family: arial;
		text-align: left;
		width: 100%;
		position: sticky;
		top: 0;
	}
	ul.topnav li {	
		float: left;
	}
	ul.topnav li a {
		display: block;
		color: white;
		text-align: center;
		padding: 14px 16px;
		text-decoration: none;
		float: left;
		font-size: 17px;
		border-right: 1px solid #bbb;
	}
	ul.topnav li a:hover:not(.active) {
		background-color: #ddd;
		color: black;
	}
	ul.topnav li a.active {
		background-color: #4CAF50;
	}
	ul.topnav li.right {
		float: right;
	}
	@media screen and (max-width: 720px) {
		ul.topnav li{
			width: 100%;
		}
		ul.topnav a{
			width: 100%;
		}
	}
</style>