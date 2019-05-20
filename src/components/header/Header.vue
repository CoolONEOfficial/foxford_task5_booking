<template>
    <!--TODO: header-->
    <v-layout row>
        <Search></Search>
        <CurrencySelection></CurrencySelection>
        <LanguageSelection></LanguageSelection>
    </v-layout>
</template>

<script>
    import CurrencySelection from "./CurrencySelection";
    import LanguageSelection from "./LanguageSelection";
    import Search from "../gray/Search";

    export default {
        name: "Header",
        components: {
            Search,
            LanguageSelection,
            CurrencySelection,
        },
    }
</script>

<style scoped lang="scss">
    @import "../../styles/colors";

    .header {
        background: red;
    }
</style>
