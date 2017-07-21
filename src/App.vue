<template>
    <div id="app">
        <Navbar/>
        <div id="wrapper" class="container-fluid">
            <br><br><br><br><br>
            <div class="row">
                <div class="offset-md-1 col-md-4">
                    <Form/>
                </div>
                <div class="row">
                    <div class="offset-md-6 col-md-8">
                        <PostContent headline="New Hampshire Decriminalizes Marijuana"/>
                        <PostContent headline="A rocket launch that looks like a squirrel ejaculating"/>
                        <PostContent headline="Team pulls off a beautiful goal despite terrible pitch conditions"/>
                        <PostContent headline="Playing 'Trump vs. Trump' never gets old."/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import Navbar from './components/Navbar.vue'
    import Form from './components/Form.vue'
    import PostContent from './components/Card.vue'

    export default {
        name:       'app',
        components: {
            Navbar,
            Form,
            PostContent
        }
    }
</script>
<style>
    PostContent {
        margin-right: 20px;
    }

    #wrapper {
        font-family: Verdana, SansSerif;
    }

</style>
