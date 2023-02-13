<template>
        <v-container fluid class="fill-height hero">
        <v-responsive class="d-flex align-center text-center fill-height">
    
            <h1 class="text-h2 font-weight-bold">RATEMYRAIDER</h1>
    
            <div class="py-2" />

            <v-text-field label="Search Players" class="searchbar" variant="outlined"></v-text-field>
    
            <v-row class="d-flex align-center justify-center">
    
            <v-col cols="auto">
                <v-btn
                @click="$router.push('Player')"
                color="primary"
                href=""
                min-width="228"
                rel="noopener noreferrer"
                size="x-large"
                target="_blank"
                variant="flat"
                >
    
                Search
                </v-btn>
            </v-col>

            </v-row>
        </v-responsive>
        </v-container>
</template>
  
<script lang="ts" setup>
    //
</script>

<style scoped>
.hero {
    background: url('../assets/Sharlayan.png')
    no-repeat center center fixed !important;
    background-size: cover;
}
.hero::before {
    content: "";
    position: absolute;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    background-color: rgba(255, 255, 255, 0.75);
}

.searchbar {
    padding-left: 10%;
    padding-right: 10%;
}
</style>
  