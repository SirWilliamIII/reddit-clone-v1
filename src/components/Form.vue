<template>
    <div>
        <form class="form">
            <div class="form-group row">
                <div class="col-sm-6 offset-sm-3 col-xl-6 offset-xl-3">
                    <label for="name" class="col-sm-1 col-form-label col-xl-1">Name: </label>
                    <input v-model="post.name" class="form-control" id="name" placeholder="">
                </div>
            </div>
            <div class="form-group row">
                <div class="col-sm-6 offset-sm-3 col-xl-6 offset-xl-3" id="">
                    <label for="categoryInput" class="col-xs-1 col-form-label">Category: </label> <input
                    v-model="post.category"
                    class="form-control" id="categoryInput" placeholder="">
                </div>
            </div>
            <div class="form-group row">
                <div class="col-sm-6">
                    <div>
                        <label>{{ postArea }}</label>
                        <textarea v-model="post.description" name="post" cols="50" rows="6" id="postArea"></textarea>
                    </div>
                </div>
            </div>


            <div class="form-group row">
                <div class="col-sm-6 offset-sm-3 col-xl-6 offset-xl-3">
                    <button @click="publishPost" type="button" class="btn btn-primary" id="submitButton">Publish
                    </button>
                    <button type="reset" class="btn btn-danger">Clear Text Area</button>
                </div>
            </div>
        </form>
    </div>
</template>

<script>
    export default {
        name:    'form',
        props:   ['onAddPost'],
        data() {
            return {
                post: {
                    name:        '',
                    category:    '',
                    description: ''
                }
            }
        },
        methods: {
            publishPost() {
                this.onAddPost({
                    name:        this.post.name,
                    category:    this.post.category,
                    description: this.post.description
                });
                this.post.name = ''
                this.post.category = ''
                this.post.description = ''
            }
        }
    }
</script>

<style>

    #name {
        padding-left: 0px;
    }
</style>
