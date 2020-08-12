<template>
    <v-app>
        <v-toolbar-items app>
            <!--color="primary"
                   dark>
            <div class="d-flex align-center">
                <v-img alt="Vuetify Logo"
                       class="shrink mr-2"
                       contain
                       src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
                       transition="scale-transition"
                       width="40" />

                <v-img alt="Vuetify Name"
                       class="shrink mt-1 hidden-sm-and-down"
                       contain
                       min-width="100"
                       src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
                       width="100" />
            </div>

            <v-spacer></v-spacer>

            <v-btn href="https://github.com/vuetifyjs/vuetify/releases/latest"
                   target="_blank"
                   text>
                <span class="mr-2">Latest Release</span>
                <v-icon>mdi-open-in-new</v-icon>
            </v-btn>-->
            <v-row>
                <v-tab to="/">Home</v-tab> |
                <v-tab to="/about">About</v-tab> |
                <v-tab to="/contact">Contact</v-tab> |
                <v-tab to="/projects">Projects</v-tab>
            </v-row>

        </v-toolbar-items>

        <v-row>
            <router-view></router-view>
        </v-row>




    </v-app>
</template>

<script>


    export default {
        name: 'App',

        components: {

        },

        data: () => ({
            //
        }),
    };
</script>


<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }

    #nav {
        padding: 30px;
    }

        #nav a {
            font-weight: bold;
            color: #2c3e50;
        }

            #nav a.router-link-exact-active {
                color: #42b983;
            }
</style>

