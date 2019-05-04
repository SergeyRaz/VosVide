<template>
	<v-app>
		<app-header/>
		<sign-up/>
		<sign-in/>
		<app-main/>
		<app-footer/>
	</v-app>
</template>

<script>
import AppHeader from "@/components/AppHeader";
import SignUp from "@/components/SignUp";
import SignIn from "@/components/SignIn";
import AppMain from "@/components/AppMain";
import AppFooter from "@/components/AppFooter";
export default {
	name: "App",
	components: { AppHeader, SignUp, SignIn, AppMain, AppFooter },
	data() {
		return {
			//
		};
	}
};
</script>
<style lang="scss">
.application--wrap {
}
</style>

