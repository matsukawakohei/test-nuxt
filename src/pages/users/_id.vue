<template>
    <div>
        <h1>ユーザID: {{ this.$route.params.id }}</h1>
        <h1>ユーザ: {{ user.name }}</h1>
    </div>
</template>

<script>
export default {
    data(){
        return {
            id: this.$route.params.id,
            users: [
                { 
                    id: 1, name: 'John Doe'
                },
                {
                    id: 2, name: 'Kevin Smith',
                },
                {
                    id: 3, name: 'Harry Bosch'
                },
            ],
        }
    },
    computed:{
        user(){
            return this.users.find(user => user.id == this.id);
        } 
    }
}
</script>