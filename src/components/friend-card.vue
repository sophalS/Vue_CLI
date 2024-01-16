<template>
  <div class="friend-card" v-for="data of myData" :key="data">
  <h3 >{{data.firstName}} {{data.lastName}}</h3>
  <span>{{data.comm}}</span>
  </div>
</template>

<script>
// import FriendForm from "./components/friend-form";

export default {
props:[
  'myData'
]

}
</script>

<style>
.friend-card{
    width: 90%;
    justify-content: center;
    margin: auto;
    padding: 2%;
    background-color: white;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    text-align: center;


}
h3,span{
  display: flex;
  justify-content: flex-start;
  font-family: sans-serif;
}
h3{
  text-transform: uppercase;
}

</style>