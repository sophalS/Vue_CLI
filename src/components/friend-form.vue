<template>
  <div class="friend-form">
  <input type="text" placeholder="First Name" v-model="first_name ">
  <input type="text" placeholder="Last Name" v-model="last_name">
  <input type="text" placeholder="Comment" v-model="comment">
  <button @click="saveData">ADD</button>
  </div>
  <card :myData="myData"></card>
</template>
<script>
import card from "./friend-card.vue"
export default {
    components:{
        card,
},
    data(){
        return {
        first_name:'',
        last_name:'',
        comment:'',
        myData:[],
    }
},
    methods:{
        saveData(){
        this.myData.push({
            firstName:this.first_name,
            lastName:this.last_name,
            comm:this.comment
            });
            this.first_name='';
            this.last_name='';
            this.comment='';
        // console.log(this.myData);
        }
    },
  
};
</script>
<style>
.friend-form{
    width: 50%;
    justify-content: center;
    margin: auto;
    padding: 2%;
    background-color: white;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
}
input{
    width: 90%;

}
button{
    background: rgb(72, 125, 204);
    width: 93%;
    border: 1px solid gray;
    color: white;

}
input,button{
    padding: 1%;
    margin: 1.5%;

}
</style>