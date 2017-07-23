<template>
    <div class="card w-75">
        <div class="panel panel-default" v-for="post in posts">
            <div class="panel-heading">
                <strong>Author: </strong>
                <h3>{{ post.name }}</h3>
            </div>
            <div class="panel-body">
                <strong>Post: </strong>
                <h1>{{ post.description }}</h1>
                <hr>
                <small><strong>Category: </strong>{{ post.category }}</small>
                <span class="pull-right">
                    <button @click="deletePost"
                            type="button"
                            class="btn btn-sm btn-danger">
                        Delete Post
                    </button>
                </span>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:    'form-posts',
        props:   ['posts', 'onDeletePost'],
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
            deletePost() {
                let post = this.post.index
                let num = 1
                this.onDeletePost(post, num)
            }
        }
    }
</script>

<style>

</style>
