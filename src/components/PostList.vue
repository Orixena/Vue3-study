<template>
    <div>
        <h3>Список пользователей</h3>
        <PostItem
            v-for="post in posts"
            :post="post"
        />
    </div>
</template>

<script>
import PostItem from './PostItem.vue';


export default {
    components: {PostItem},
    props: {
        posts: {
            type: Array,
            required: true
        }
    },
    components: { PostItem, PostItem, PostItem }
}

</script>

<style scoped>

</style>