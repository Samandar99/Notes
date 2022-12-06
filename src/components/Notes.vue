<template>
  <div class="notes">
    <div class="container">
      <div class="notes__top">
        <h2 class="notes__title">All Notes</h2>
        <button class="notes__btn" @click="grid = !grid">
          <i class="fa-solid fa-bars humber fa-lg" v-if="grid"></i>
          <i class="fa fa-th fa-lg gird" v-else></i>
          <span>list</span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
        grid: true,
        
    };
  },
};
</script>

<style scoped>
.humber {
  color: #8a2be2;
}
.gird{
    color: #8a2be2;
}

.notes {
  margin-top: 30px;
}

.notes__top {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.notes__title {
  font-size: 22px;
  line-height: 28px;
  color: #323232;
}

.notes__btn {
  background: linear-gradient(
    0deg,
    rgba(103, 80, 164, 0.11),
    rgba(103, 80, 164, 0.11),
    #fffbfe
  );
  box-shadow: 0px 4px 8px 3px rgba(0, 0, 0, 0.15),
    0px 1px 3px rgba(0, 0, 0, 0.3);
  border-radius: 16px;
  cursor: pointer;
  width: 120px;
  height: 56px;
  border: none;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.notes__btn span {
  color: #6750a4;
  font-size: 16px;
  line-height: 20px;
  font-family: "RM";
}
</style>