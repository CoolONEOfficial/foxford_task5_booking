<template>
    <div id="app">
        <v-layout class="header-wrapper" row justify-center>
            <v-flex class="header" xs7>
                <Header></Header>
            </v-flex>
            <!-- /.header -->
        </v-layout>
        <!-- /.header-wrapper -->

        <v-layout row justify-center class="gray-wrapper">
            <v-flex class="gray" xs7>
                <!--TODO: all gray here (search, date and customer picker)-->
                <!--use:-->
                <HousingPicker></HousingPicker>
                <DatePicker></DatePicker>
                <Search></Search>
            </v-flex>
            <!-- /.search -->
        </v-layout>
        <!-- /.search-wrapper -->

        <v-layout row justify-center class="body-wrapper">
            <v-flex class="body" xs7>

                <div class="popupad-wrapper">
                    <PopUpAd></PopUpAd>
                </div>
                <!-- /.popupad-wrapper -->

                <h2 class="housing-slider__title">
                    5.7 million homes, big or small… and you thought we only did hotels
                </h2>
                <HousingSlider></HousingSlider>

                <h2 class="places-grid__title">
                    Get inspiration for your next trip
                </h2>
                <PlacesGrid></PlacesGrid>

                <h2 class="travellers-slider__title">
                    Connect with other travellers
                </h2>
                <TravellersSlider></TravellersSlider>

                <h2 class="hotels-slider__title">
                    More than just hotels…discover pure comfort with homes & apartments
                </h2>
                <HotelsSlider></HotelsSlider>

                <h3 class="hotels-slider__title">
                    Destinations we love
                </h3>
                <DestinationsSlider></DestinationsSlider>

                <LovedDestinations></LovedDestinations>

                <DiscoverCountries></DiscoverCountries>

            </v-flex>
            <!-- /.body -->
        </v-layout>
        <!-- /.body-wrapper -->

        <v-layout row justify-center class="subscribe-form-wrapper">
            <v-flex class="subscribe-form" xs7>
                <SubscribeForm></SubscribeForm>
            </v-flex>
            <!-- /.subscribe-form -->
        </v-layout>
        <!-- /.subscribe-form-wrapper -->

        <v-layout row justify-center class="partners-wrapper">
            <v-flex class="partners" xs7>
                <Partners></Partners>
            </v-flex>
            <!-- /.partners -->
        </v-layout>
        <!-- /.partners-wrapper -->

        <div style="height: 1px; background: #537bb4;"></div>

        <v-layout row justify-center class="top-footer-wrapper">
            <v-flex class="top-footer" xs7>
                <TopFooter></TopFooter>
            </v-flex>
            <!-- /.top-footer -->
        </v-layout>
        <!-- /.top-footer-wrapper -->

        <v-layout row justify-center class="bottom-footer-wrapper">
            <v-flex class="bottom-footer" xs7>
                <BottomFooter></BottomFooter>
            </v-flex>
            <!-- /.bottom-footer -->
        </v-layout>
        <!-- /.bottom-footer-wrapper -->

        <CookieMessage></CookieMessage>

        <!--v-layout[row justify-center].search-wrapper>v-flex.search[xs7]|c-->
    </div>
</template>

<script>
    import CookieMessage from './components/CookieMessage';
    import DatePicker from './components/gray/DatePicker';
    import BottomFooter from './components/footer/BottomFooter';
    import Header from './components/header/Header';
    import HousingSlider from './components/body/HousingSlider';
    import LovedDestinations from './components/body/LovedDestinations';
    import PlacesGrid from './components/body/PlacesGrid';
    import PopUpAd from './components/body/PopUpAd';
    import Search from './components/gray/Search';
    import SubscribeForm from './components/footer/SubscribeForm';
    import DestinationsSlider from "./components/body/DestinationsSlider";
    import TravellersSlider from "./components/body/TravellersSlider";
    import HotelsSlider from "./components/body/HotelsSlider";
    import DiscoverCountries from "./components/body/DiscoverCountries";
    import Partners from "./components/footer/Partners";
    import TopFooter from "./components/footer/TopFooter";

    export default {
        name: 'app',
        components: {
            TopFooter,
            BottomFooter,
            Partners,
            DiscoverCountries,
            HotelsSlider,
            CookieMessage,
            DatePicker,
            Header,
            HousingSlider,
            LovedDestinations,
            PlacesGrid,
            PopUpAd,
            Search,
            SubscribeForm,
            DestinationsSlider,
            TravellersSlider,
        }
    }
</script>

<style lang="scss">
    @import "styles/colors";

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
    }

    .header-wrapper {
        height: 110px;
        background: $primary;
    }

    .gray-wrapper {
        height: 260px;
        background: #f7f7f7;
    }

    .popupad-wrapper {
        padding: 24px;
        margin-top: 24px;
        margin-bottom: 24px;
        border: 1px solid #e0e0e0;
        border-radius: 2px;
    }

    .subscribe-form-wrapper {
        height: 253px;
        background: $primary-dark;
    }

    .partners-wrapper {
        height: 60px;
        background: $primary;
    }

    .top-footer-wrapper {
        height: 44px;
        background: $primary;
    }

    .bottom-footer-wrapper {
        height: 253px;
    }

    .housing-slider__title {
        padding-top: 1.5em;
        font-size: 20px;
        font-weight: 600;
        line-height: 28px;
        margin-left: 0;
        margin-bottom: 10px;
    }

    .places-grid__title {
        margin: 20px 0;
        font-size: 24px;
        line-height: 32px;
        font-weight: 600;
    }

    .travellers-slider__title {
        font-size: 20px;
        line-height: 28px;
        font-weight: 500;
        margin: 0 0 16px;
    }

    .hotels-slider__title {
        font-size: 140%;
        font-weight: bold;
        padding: 16px 0;
    }

    .destinations-slider__title {

    }
</style>
