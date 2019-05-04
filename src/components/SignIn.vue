<template>
	<form class="sign-in">
		<v-text-field class="sign-in-email-field" label="Ваш Email" placeholder></v-text-field>
		<v-text-field class="sign-in-email-password" label="Ваш Пароль" placeholder></v-text-field>
		<v-btn small color="primary">Войти</v-btn>
	</form>
</template>
<script>
export default {
	name: "SignIn"
};
</script>
<style lang="scss">
.sign-in {
	padding: 30px;
	.v-btn {
		margin-left: 0;
	}
}
</style>