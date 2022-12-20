<template>
  <div class="modal" @click="closeModal">
    <div class="modal__block" @click.stop="">
      <h2 class="modal__title">add Note</h2>
      <div class="modal__inputs">
        <label>
          <span>Title</span>
          <input type="text" />
        </label>
        <label>
          <span>Content</span>
          <textarea></textarea>
        </label>
      </div>
      <div class="modal__btns">
        <button class="modal__btn cancel" @click="closeModal">cancel</button>
        <button class="modal__btn add">add</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    closeModal(){
      this.$emit('closeModal',false)  
    }
  
  }
};
</script>

<style>
.modal {
  background: rgba(0, 0, 0, 0.35);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 9999;
  display: flex;
  justify-content: center;
  align-items: center;
}
.modal__block {
  background: linear-gradient(
      0deg,
      rgba(103, 80, 164, 0.11),
      rgba(103, 80, 164, 0.11)
    ),
    rgb(248, 248, 242);
  border-radius: 28px;
  max-width: 312px;
  width: 100%;
  padding: 24px;
}

.modal__title {
  color: #1c1b1f;
  font-size: 24px;
  line-height: 32px;
  margin-bottom: 16px;
}
.modal__inputs {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.modal__inputs label {
  position: relative;
}
.modal__inputs span {
  position: absolute;
  left: 16px;
  top: 8px;
  font-size: 12px;
  line-height: 16px;
  color: #6750a4;
}

.modal__inputs input,
.modal__inputs textarea {
  background: #e7e0ec;
  border-radius: 4px;
  width: 100%;
  border: none;
  outline: none;
  padding: 23px 0 9px 16px;
  font-size: 16px;
  line-height: 24px;
  color: #49454f;
  border-bottom: 1px solid #1c1b1f;
  resize: none;
}

.modal__btns {
  display: flex;
  justify-content: flex-end;
  gap: 10px;
  margin-top: 25px;
}
.modal__btn {
  font-size: 14px;
  line-height: 20px;
  font-family: "RM";
  background: transparent;
  padding: 10px 12px;
  border: none;
  cursor: pointer;
  text-transform: uppercase;
  transition: background 500ms;
}
.cancel {
  color: #cf1b1b;
}

.cancel:hover{
    background: #FFE1E1;
}
.add {
  color: #6750a4;
}

.add:hover{
    background: #E6DDFF;
}

</style>