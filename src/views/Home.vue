<template>
    <div>
        <h1>Welcome to {{title2}}!</h1>
        <input type="text" v-model="input1"/>
        <button type="button" @click="getData">Get</button>
        <button type="button" @click="setData">Set</button>
    </div>
</template>

<script>
export default {
    data(){
        return {
            title: "개발자의 품격",
            title2: "Seoul",
            input1: "abcde",
        };
    },
    methods: {
        getData(){
            alert(this.input1);
        },
        setData(){
            this.input1="1234";
        }
    },

}
</script>