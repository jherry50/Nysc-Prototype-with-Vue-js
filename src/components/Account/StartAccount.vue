<template>
        <div class="row">
            <div class="col-lg-7">
                <img src="../../assets/carousel.jpeg" alt="A create picture" class="img-fluid" style="max-height:750px"/>
            </div>
            <div class="col-lg-5 confStart ">
                <confirmEmail v-if="step===1" @stepPlus="step= $event"/>
                <create-account v-if="step===2" @stepMinus="step= $event"/>
            </div>
        </div>
        
</template>

<script>
import confirmEmail from "./ConfirmMail"
import createAccount from "./CreateAccount"
export default {
    data () {
        return{
            step:1
        }
    },
    components: {
        confirmEmail,
        createAccount

    }
    
}
</script>

<style scoped>
.confStart {
    margin: auto;
}

</style>