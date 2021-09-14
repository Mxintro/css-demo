<template>
	<div class="tab-navbar-component">TabNavbar Component {{done}}</div>
</template>

<style lang="scss">
.tab-navbar-component {
	font-size: 20px;
	color: #f66;
}
</style>

<script>
export default {
	name: "tab-navbar",
	props: {
		done: {
			default: "Done",
			type: String
		}
	}
};
</script>