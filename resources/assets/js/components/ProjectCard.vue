<template>
    <div class="card project-card">
        <div class="card-content">
            <div class="media">
                <div class="media-left">
                    <figure class="image is-48x48">
                        <img src="https://bulma.io/images/placeholders/96x96.png" alt="Placeholder image">
                    </figure>
                </div>
                <div class="media-content">
                    <p class="title is-4">{{title}}</p>
                    <p class="subtitle is-6">@{{user}}</p>
                </div>
            </div>

            <div class="content" v-html="content">
                {{ content }}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "projectcard",
        props: ['title', 'user', 'content']
    }
</script>

<style scoped>
.project-card {
    margin-bottom: 40px;
}
</style>