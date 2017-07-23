<template>
    <nav class="navbar navbar-toggleable-xs bg-info">
        <div class="container-fluid">
            <div class="row">
                <a class="navbar-brand" href="#" id="logo"> <img height="48" width="48" src="../assets/logo.png" alt="">
                </a>
                <span class="navbar-text center-block" style="color: red">
                    <h3>{{ title }}</h3>
                </span>
            </div>
        </div>
    </nav>
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
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #333;
    }

    #logo {
        margin-left: 10px;
    }


</style>
