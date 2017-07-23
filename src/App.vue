<template>
    <div id="app">
        <div id="wrapper" class="container-fluid">
            <Navbar/>
            <main>
                <FormPosts/>
            </main>
        </div>
    </div>
</template>

<script>
    import Navbar from './components/Navbar'
    import FormPosts from './components/Form-posts'

    export default {
        name:       'app',
        components: {
            Navbar,
            FormPosts
        }
    }
</script>
<style>
    #wrapper {
        font-family: "Verdana", SansSerif;
    }
</style>
