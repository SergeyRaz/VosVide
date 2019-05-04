<template>
	<div class="app-footer">
		<v-btn color="primary" fab small dark>
			<v-icon>skip_previous</v-icon>
		</v-btn>
		<v-btn color="primary" fab small dark>
			<v-icon>play_arrow</v-icon>
		</v-btn>
		<v-btn color="primary" fab small dark>
			<v-icon>skip_next</v-icon>
		</v-btn>
	</div>
</template>
<script>
export default {
	name: "AppFooter"
};
</script>
<style lang="scss">
.app-footer {
	padding: 15px 20px;
	box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
	position: fixed;
	left: 0;
	right: 0;
	bottom: 0;
	display: grid;
	grid-template-columns: min-content min-content min-content;
	justify-content: center;
}
</style>