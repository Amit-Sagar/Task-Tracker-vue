<template>
  <header>
    <h1>{{title}}</h1>
    <Button @btn-click="$emit('toggle-btn')" :text="showBox?'Close':'Add Task'" :color="showBox?'red':'green'"/>
  </header>
</template>
<script>
import Button from './Button'
export default {
    name: "Header",
    components:{
     Button,
    },
  props: {
    title: String,
    showBox: Boolean,
  },
};
</script>

<style scoped>
header{
 display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  }
</style>
