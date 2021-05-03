<template>
  <v-app>


      <!-- V-card used to make a container -->
      <v-card width="400" class="mx-auto mt-5">
        <!-- v-card-title used to make sure the component has the right space and positions -->
        <v-card-title>
          <h1 class="display-1">Login</h1>
        </v-card-title>
        <!-- v-card-text it's like the body -->
        <v-card-text>
          <!-- v-form used to wrap the content -->
          <v-form>

            <!-- input field -->
            <v-text-field 
              prepend-icon="mdi-account-circle" 
              label="Username"/>


<v-text-field
prepend-icon="mdi-lock" 
  id="password"
  name="password"
  label="Password" 
  :type="show ? 'text':'Password'"
  :append-icon="show ?'mdi-eye':'mdi-eye-off'" 
  @click:append="show=!show"

>
</v-text-field>

          </v-form>

        </v-card-text>

        <v-divider></v-divider>
        <!-- this component for the calls that we will make -->
        <v-card-actions>

          <v-btn color="success">Register</v-btn>
          <v-spacer></v-spacer>
          <v-btn color="info">Login</v-btn>

        </v-card-actions>

      </v-card>

    
  </v-app>
</template>

<script>
export default {
	name: 'App',
	data() {
		return {
			show: false
		}
	}
}
</script>
