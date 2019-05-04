<template>
	<div class="app-header">
		<v-btn class="app-header-logo" color="primary" fab dark small>
			<v-icon>extension</v-icon>
		</v-btn>
		<v-btn small color="primary">Войти</v-btn>
		<v-btn small color="primary">Зарегистрироваться</v-btn>
	</div>
</template>
<script>
export default {
	name: "AppHeader"
};
</script>
<style lang="scss">
.app-header {
	padding: 15px 20px;
	box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
	display: grid;
	grid-template-columns: 1fr min-content min-content;
	justify-content: end;
	align-items: center;
	.app-header-logo {
		align-self: start;
	}
}
</style>