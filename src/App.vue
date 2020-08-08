<template>
    <div id="app">
        <navigation v-bind:currentDisplay="currentDisplay" @navSelection="currentDisplay = $event"></navigation>
        <about v-if="currentDisplay == 'About'"></about>
        <contact v-if="currentDisplay == 'Contact'"></contact>
        <home v-if="currentDisplay == 'Home'"></home>
        <projects v-if="currentDisplay == 'Projects'"></projects>
    </div>
</template>

<script>
    import navigation from './components/Navigation.vue';
    import about from './components/About.vue';
    import contact from './components/Contact.vue';
    import home from './components/Home.vue';
    import projects from './components/Projects.vue';

    export default {
        name: 'App',
        data: function () {
            return {
                currentDisplay: 'Home'
            }
        },
        components: {
            navigation,
            about,
            contact,
            home,
            projects
        }
    }
</script>

<style>

    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
