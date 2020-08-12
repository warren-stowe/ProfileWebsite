<template>
    <v-container>
        <h1 class="text-decoration-underline ma-8">CONTACT</h1>

        <h3 class="mb-6">[ PLACEHOLDER FOR SOMETHING WITTY ]</h3>

        <v-row class="d-flex justify-center">
            <v-text-field autofocus outlined filled label="Name" class="formWidth"></v-text-field>
        </v-row>
        <v-row class="d-flex justify-center">
            <v-text-field outlined filled label="Email" class="formWidth"></v-text-field>
        </v-row>
        <v-row class="d-flex justify-center">
            <v-textarea outlined filled label="Message" class="formWidth"></v-textarea>
        </v-row>
        <v-row class="d-flex justify-center">
            <v-btn dark color="blue">Send</v-btn>
        </v-row>

    </v-container>
</template>

<script>
    export default {

    }
</script>


<style>
    .formWidth {
        max-width: 500px;
    }
</style>