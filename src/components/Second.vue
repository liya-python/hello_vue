<template>
    <div>
        <p>
            这是我的第二个组件
        </p>
        {{username}}
        <hr>
        <span v-model="count">{{count}}</span>
        <button @click="change">按钮</button>
    </div>
</template>

<script>
    export default {
        name: "Second",
        data:function () {
            return {
                username:'小黑',
                count:80,
            }
        },
        methods:{
            change(){
                // alert('触发了事件');
                this.count--;
            }
        }
    }
</script>

<style scoped>

</style>
