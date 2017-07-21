<template>
    <div class="navigation">
        <nav class="navbar fixed-top navbar-inverse bg-info">
            <div class="row">
                <a class="navbar-brand" href="#" id="logo"><img src="../assets/logo.png" alt=""></a>
                <div id="title">
                    <span class="navbar-text" style="color: white">
                        <h1>{{ title }}</h1>
                    </span>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        name:    'navigation',
        data() {
            return {
                title: 'A title, ah, but a label'
            }
        },
        methods: {}
    }
</script>

<style>
    #title {
        margin: auto;
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;

    }

    #logo {
        margin-left: 10px;
    }


</style>