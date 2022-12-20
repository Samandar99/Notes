<template>
  <button class="add__btn" @click="$emit('openModal')">
    <i class="fa fa-pencil pen"></i>
  </button>
</template>

<script>
export default {

}
</script>

<style>
.add__btn{
    background: linear-gradient(0deg, rgba(103,80,164,0.11),rgba(103,80,164,0.11));
    border-radius: 16px;
    cursor: pointer;
    width: 56px;
    height: 56px;
    border: none;
    position: fixed;
    right: 30px;
    bottom: 30px;
}
.pen{
    color: #6750a4;
}

</style>