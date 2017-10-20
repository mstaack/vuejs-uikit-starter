<template>
    <div id="app">
        <!--HEADER-->
        <header>
            <nav class="uk-navbar-container">
                <div class="uk-container">
                    <div class="uk-navbar">
                        <div class="uk-navbar-left">
                            <a class="uk-navbar-item uk-logo" href="#">Logo</a>

                        </div>
                        <div class="uk-navbar-center">
                            <ul class="uk-navbar-nav">
                                <li class="uk-active"><a href="#">Active</a></li>
                                <li><a href="#">Item</a></li>
                                <li><a href="#">Item</a></li>
                                <li><a href="#">Item</a></li>
                            </ul>
                        </div>
                        <div class="uk-navbar-right">
                            <div>
                                <a class="uk-navbar-toggle" uk-search-icon href="#"></a>
                                <div class="uk-drop" uk-drop="mode: click; pos: left-center; offset: 0">
                                    <form class="uk-search uk-search-navbar uk-width-1-1">
                                        <input class="uk-search-input" type="search" placeholder="Search for images"
                                               autofocus>
                                    </form>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </nav>
        </header>
        <!--/HEADER-->

        <router-view/>

        <!--FOOTER-->
        <footer class="uk-section uk-section-default uk-section-small">
            <div class="uk-container">
                <p class="uk-text-small uk-text-center">
                    Copyright 2017 - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus hendrerit tristique tortor vel ultricies. </p>
            </div>
        </footer>
        <!--/FOOTER-->
    </div>
</template>

<script>
  export default {
    name: 'app'
  }
</script>

<style lang="scss">

    // 1. Your custom variables and variable overwrites.
    $global-link-color: #DA7D02;

    // 2. Import default variables and available mixins.
    @import "~uikit/src/scss/variables-theme.scss";
    @import "~uikit/src/scss/mixins-theme.scss";

    // 3. Your custom mixin overwrites.
    @mixin hook-card() {
        color: #000;
    }

    // 4. Import UIkit.
    @import "~uikit/src/scss/uikit-theme.scss";

    // Some font smoothing
    html {
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-rendering: optimizeLegibility;
    }
</style>
