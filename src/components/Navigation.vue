<template>


    <nav>
        <h2>THIS IS THE NAV BAR</h2>
        <ul>
            <li>
                <h2 @click="updateDisplay('Home')">Home</h2>
            </li>
            <li>
                <h2 @click="updateDisplay('About')">About</h2>
            </li>
            <li>
                <h2 @click="updateDisplay('Projects')">Projects</h2>
            </li>
            <li>
                <h2 @click="updateDisplay('Contact')">Contact</h2>
            </li>
        </ul>
    </nav>
</template>



<script>
    export default {
        methods: {
            updateDisplay: function (update) {
                this.$emit('navSelection', update);
            }
        }
    }


</script>