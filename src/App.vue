<template>
  <Navbar />
  <Notes :notes="notes" />
  <Modal v-show="modalOpen" @closeModal="closeModal"/>
  <AddButton @openModal="openModal"/>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Notes from "@/components/Notes.vue";
import Modal from "@/components/Modal.vue";
import AddButton from "@/components/AddButton.vue";


export default {
  components: {
    Navbar,
    Notes,
    Modal,
    AddButton,
  },
  data() {
    return {
      modalOpen: false,
      notes: [
        {
          id: 1,
          title: "Vue",
          descr: "Lorem ipsum dolor sit amet.",
          date: "07.07.2022",
        },
        {
          id: 2,
          title: "React",
          descr: "Lorem ipsum dolor sit amet.",
          date: "07.07.2022",
        },
        {
          id: 3,
          title: "Angular",
          descr: "Lorem ipsum dolor sit amet.",
          date: "07.07.2022",
        },
      ],
    };
  },
  methods: {
    openModal() {
      this.modalOpen = true
    },
    closeModal(status){
      this.modalOpen = status
    }
  }
  
};
</script>

<style>
</style>
