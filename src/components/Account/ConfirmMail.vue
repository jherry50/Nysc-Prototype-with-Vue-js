<template>
    <div class="container">
        <div>
            <h4>Confirm your mail</h4>
            <hr>
            <form action="#" role="form">
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" class="form-control">
                </div>
                <button class="btn btn-success" @click="chgStp">Confirm</button>
                <p class="text-warning mt-4"> kindly check your mail for verificaion link</p>
                
            </form>
        </div>

    </div>
</template>

<script>
export default {
    data(){
        return{
            step: 1,
        }
    },
    methods: {
        chgStp(){
            this.step +=1
            this.$emit('stepPlus', this.step)
        }
    }
    
}
</script>

<style scoped>
.container{
    max-width:30em;
    border: 1px solid rgba(0, 128, 0, 0.137);
    box-shadow: 0 2px 3px rgb(215, 243, 222);
    padding: 50px;
    font-size:14px;
}

</style>