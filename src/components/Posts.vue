<template>
    <section>
        <div class="card w-75">
            <div class="panel panel-default" v-for="post in posts">
                <div class="panel-heading">{{ post.name }}</div>
                <div class="panel-body">
                    {{ post.description }}
                    <small>{{ post.category }}</small>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name:    'form-posts',
        props: ['posts']
    }
</script>

<style>

</style>
