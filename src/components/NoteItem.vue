<template>
  <div class="notes__item">
    <div class="notes__item-top">
      <h3 class="notes__item-title">Title</h3>
      <p class="notes__item-date">07.03.2022</p>
    </div>
    <p class="notes__item-text">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cumque,
      molestias omnis.
    </p>
    <div class="notes__item-btns">
      <button class="notes__item-btn edit">
        <i class="fa-solid fa-pencil icon-pen"></i>
        <span>Edit</span>
      </button>
      <button class="notes__item-btn del">
        <i class="fa fa-trash icon-pen"></i>
        <span>Edit</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.notes__item {
  background: linear-gradient(
      0deg,
      rgba(103, 80, 164, 0.05),
      rgba(103, 80, 164, 0.05)
    )
    #fffbfe;
  box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.3),
    0px 1px 3px 1px rgba(0, 0, 0, 0.15);
  border-radius: 16px;
  padding: 16px 16px 28px 16px;
}

.icon-pen {
  color: #8a2be2;
}

.notes__item-title{
  font-size: 16px;
  line-height: 24px;
  font-family: 'RM';
}

.notes__item-date{
  color: #CAC4D0;
  font-size: 14px;
  line-height: 20px;
  letter-spacing: 0.25px;
}
.notes__item-text{
  font-size: 14px;
  line-height: 20px;
  color: #49454F;
  margin-bottom: 20px;  
  margin-top: 20px;
}
.notes__item-btns{
  display: flex;
  justify-content: flex-end;
  gap: 15px;
}
.notes__item-btn{
  display: flex;
  align-items: center;
  gap: 10px;
  background: transparent;
  border: none;
  padding: 12px;
  border-radius: 5px;
  
}

.notes__item-btn span{
  font-size: 14px;
  line-height: 20px;
  font-family: 'RM';

}

.edit{
  color: #8a2be2;
}
.edit:hover{
  background: #E6DDFF;
}

.del{
  color: #CF1B1B;
}
.del:hover{
  background: #FFE1E1;
}


</style>