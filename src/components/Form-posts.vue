<template>
    <div>
        <Form
            :onAddPost="onAddPost"
        ></Form>
        <br>
        <PostContent
            :posts="posts"
        ></PostContent>
    </div>
</template>

<script>
    import Form from './Form.vue'
    import PostContent from './Posts.vue'
    import posts from '../lib/posts'

    export default {
        name:       'form-posts',
        components: {
            Form,
            PostContent
        },
        data() {
            return {
                message: '',
                posts
            }
        },
        methods:    {
            onAddPost(post) {
                this.posts.push(post)
            }
        }
    }
</script>

<style>

</style>
