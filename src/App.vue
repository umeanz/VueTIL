<template>
<button @click="add">ADD</button>
    <h1>
        {{reversedMessage}}
    </h1>
</template>

<script>
export default {
    data() {
        return {
            msg: 'Hello Compute!'
        }
    },
    computed: {
        // reversedMessage(){
        //     return this.msg.split('').reverse().join('')
        // }
        reversedMessage:{
            get() {
                return this.msg.split('').reverse().join('')
            },
            set(newValue){
                this.msg = newValue
            }
        }
    },
    methods: {
        add(){
            this.reversedMessage += '!?'
        },
        // reverseMessage(){
        //     return this.msg.split('').reverse().join('')
        // }
    }
}
</script>