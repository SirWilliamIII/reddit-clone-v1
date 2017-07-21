<template>
    <div class="offset-xs-4 col-xs-4">
        <div class="postContent">
            <div class="card w-75">
                <div class="card-block">
                    <h4 class="card-title">{{ headline }}</h4>
                    <p class="card-text">category: trending</p>
                    <a href="#" class="btn btn-sm btn-success">View full
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:    'postContent',
    data() {
        return {
            message: '',
            items:   [{}, {}, {}]
        }
    },
    methods: {
        methodName: function () {

        }
    },
    props: ['headline']
}
</script>

<style>

</style>
