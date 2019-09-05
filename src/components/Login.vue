<template>
    <v-app>
        <v-content>
				<v-container class="fill-height" fluid>
						<v-row align="center" justify="center">
							<v-col
								cols="12"
								sm="8"
								md="4"
							>
								<v-card class="elevation-12">
									<v-toolbar
										color="primary"
										dark
										flat
									>
										<v-toolbar-title>Login form</v-toolbar-title>
									</v-toolbar>
									<v-card-text>
										<v-form>
											<v-text-field
												label="Login"
												name="login"
												prepend-icon="person"
												type="text"
											></v-text-field>

											<v-text-field
												id="password"
												label="Password"
												name="password"
												prepend-icon="lock"
												type="password"
											></v-text-field>
										</v-form>
									</v-card-text>
									<v-card-actions>
										<div class="flex-grow-1"></div>
										<router-link to="/about"><v-btn color="primary">Login</v-btn></router-link>
									</v-card-actions>
								</v-card>
							</v-col>
					</v-row>
				</v-container>
    </v-content>
  </v-app>
</template>
<script>
export default {
	
}
</script>
<style lang="scss" scoped>
#app{
  background-color:#99c4ee;
}
</style>