<template>
    <div>
        <Form
            :onAddPost="onAddPost"
        ></Form>
        <br>
        <PostContent
            :posts="posts"
            :onDeletePost="onDeletePost"
        ></PostContent>
    </div>
</template>

<script>
    import Form from './RegisterForm.vue'
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
                posts
            }
        },
        methods:    {
            onAddPost(post) {
                this.posts.push(post)
            },
            onDeletePost(post, num) {
                posts.slice(post, num)
            }
        }
    }
</script>

<style>

</style>
