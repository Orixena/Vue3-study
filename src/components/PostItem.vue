<template>
    <div class="post">
        <div>
            <div><strong>Название:</strong> {{ post.title }}</div>
            <div><strong>Описание:</strong> {{ post.body }}</div>
        </div>
        <div class="post__btns">
            <MyButton>Удалить</MyButton>
        </div>
        
    </div>
</template>

<script>
import MyButton from './UI/MyButton.vue';
export default {
    components: {MyButton},
    props: {
        post: {
            type: Object,
            required: true
        }
    },
    components: { MyButton }
}

</script>

<style scoped>
.post {
    padding: 15px;
    border: 2px solid teal;
    margin-top: 15px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

</style>