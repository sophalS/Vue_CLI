<template>
<section>
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
}
.friend-form,.friend-card{
  margin-top: 4%;
  border-radius: 5px;
}
</style>
