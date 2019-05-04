<template>
	<form class="sign-up" @submit.prevent="registerUser">
		<v-text-field
			class="sign-up-email-field"
			label="Ваш Email"
			placeholder
			:counter="50"
			data-vv-name="email"
			v-model="user.email"
			v-validate="'required|max:50|email'"
			:error-messages="errors.collect('email')"
		></v-text-field>
		<v-text-field
			class="sign-up-email-password"
			label="Ваш Пароль"
			placeholder
			type="password"
			:counter="50"
			data-vv-name="password"
			v-model="user.password"
			v-validate="'required|max:50|min:6'"
			:error-messages="errors.collect('password')"
		></v-text-field>
		<v-text-field
			class="sign-up-email-confirm"
			label="Подтвердите Пароль"
			placeholder
			type="password"
			v-model="user.confirmPassword"
			:counter="50"
			data-vv-name="confirmPassword"
			v-validate="'required|max:50|min:6'"
			:error-messages="errors.collect('confirmPassword')"
		></v-text-field>
		<div class="sign-up-error" v-if="error">Ошибка</div>
		<v-btn small color="primary">Зарегистрироваться</v-btn>
	</form>
</template>
<script>
export default {
	name: "SignUp",
	data() {
		return {
			error: false,
			user: {
				email: "",
				password: "",
				confirmPassword: ""
			}
		};
	},
	methods: {
		registerUser() {}
	}
};
</script>
<style lang="scss">
.sign-up {
	padding: 30px;
	.sign-up-error {
		color: red;
	}
	.v-btn {
		margin-left: 0;
	}
}
</style>


