<template>
<section >
<FriendNav/>
<FriendForm/>
</section>

</template>

<script>
import FriendNav from "./components/friend-nav";
import FriendForm from "./components/friend-form";

export default {
  components: {
   FriendNav,
   FriendForm,
  }
}
</script>

<style>
#app {
  justify-content: center;
  text-align: center;
  margin: auto;
  width: 50%;
  padding: 4%;
  background-color: rgb(207, 224, 224);
  border-radius: 5px;
  box-shadow: 2px 5px 10px 0 rgb(5, 5, 5);
}
.friend-form,.friend-card{
  margin-top: 4%;
  border-radius: 5px;
}
</style>
