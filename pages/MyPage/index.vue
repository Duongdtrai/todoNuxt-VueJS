<template>
    <div id = "root">
        <div>Đây là số: {{number}}</div>
        <button @click="showNumber"></button>
    </div>
</template>

<script>

export default ({
    name: "MyPage",
    data(){
        return {
            number: 1
        }
    },
    methods: {
        showNumber(){
            this.$router.push(`/MyPage/${this.number}`) // đây là việc thay đổi đường dẫn bằng thuộc tính push
        }
    },

})
</script>

