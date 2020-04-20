<template>
    <div class="project-item" v-bind:class="{'is-active':!project.active}">
        <h3>
            <input type="image" v-on:click="gotoURL" v-bind:alt="project.title + ' logo'" v-bind:src="require('../../assets/'
                + this.project.title.trim().toLowerCase() + '_logo.png')" width = 400 height = 300>
        </h3>
    </div>
</template>

<script>

export default {
    name: "ProjectItem",
    props: ["project"],
    methods: {
        gotoURL() {
            this.$router.push("/projects/" + this.project.title.trim().toLowerCase())
        },
    },
}
</script>

<style scoped>
.project-item {
    background: #f4f4f4;
    padding: 10px;
    border-bottom: 1px #ccc dotted;
}

.is-active {
    text-decoration: line-through;
}
</style>