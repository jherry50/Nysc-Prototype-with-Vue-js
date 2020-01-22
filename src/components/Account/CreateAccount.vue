<template>
    <div class="container">
        <div>
            <h4>Create your Account</h4>
            <hr>
            <form action="#" role="form">
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" class="form-control">
                </div>
                <div class="form-group">
                    <label for="confirmEmail">Email</label>
                    <input type="email" id="confirmEmail" class="form-control">
                </div>
                <div class="form-group">
                    <label for="password">Password</label>
                    <input type="password" id="password" class="form-control" required>
                </div>
                <div class="form-group">
                    <label for="confirmPassword">Confirm Password</label>
                    <input type="password" id="confirmPassword" class="form-control" required>
                </div>
                <button class="btn btn-success" @click="chgStp"> Create Account</button>
                
            </form>
        </div>
        
    </div>

</template>

<script>
export default {
    data(){
        return{
            step: 2,
        }
    },
    methods: {
        chgStp(){
            this.step -=1
            this.$emit('stepMinus', this.step)
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