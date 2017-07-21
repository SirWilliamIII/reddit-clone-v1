<template>
    <div class="form">
        <form>
            <div class="form-group row">
                <label for="nameInput" class="col-xs-1 col-form-label">{{name}}</label>
                <div class="col-sm-6 offset-sm-3" id="iname">
                    <input class="form-control" id="nameInput" placeholder="your name">
                </div>
            </div>
            <div class="form-group row">
                <label for="categoryInput" class="col-xs-1 col-form-label">{{ category }}</label>
                <div class="col-sm-6 offset-sm-2" id="icategory">
                    <input class="form-control" id="categoryInput" placeholder="category">
                </div>
            </div>
            <div class="form-group row">
                <label>{{ postArea }}</label>
                <div class="col-sm-6">
                    <div>
                        <textarea name="post" id="" cols="51" rows="6" id="postArea"></textarea>
                    </div>
                </div>
            </div>
            <div class="form-group row">
                <div class="offset-sm-4 col-sm-8">
                    <button type="submit" class="btn btn-primary" id="submitButton">Publish</button>
                    <button type="reset" class="btn btn-danger">Clear Text Area</button>
                </div>
            </div>
        </form>
    </div>
</template>

<script>
    export default {
        name:    'form',
        data() {
            return {
                message:  '',
                name:     'Name: ',
                category: 'Category: ',
                postArea:     'Write your post here: ',
                items:    [{}, {}, {}]
            }
        },
        methods: {
            publishPost: function () {
                const submitButton = document.getElementById('submitButton')
                const postArea = document.getElementById('postArea')
                const nameArea = document.getElementById('nameArea')

                if (postArea.value !== '') {

                }
            }
        }
    }
</script>

<style>
    #icategory {
            padding-left: 20px;
    }
    #iname {
        padding-left: 0px;
    }


</style>