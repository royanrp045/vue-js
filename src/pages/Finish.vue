<template>
  <div class="card rounded-3 shadow-sm">
    <Header title="Finish Task" />

    <div class="card-body px-4 border-top">
      <Navigation />
      <ItemList :todos="todos" />
    </div>

    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Navigation from "../components/Navigation.vue";
import ItemList from "../components/ItemList.vue";
import Footer from "../components/Footer.vue";

export default {
  components: {
    Header,
    Navigation,
    ItemList,
    Footer,
  },

  data() {
    return {
      todos: [
        {
          text: "Belajar HTML",
          status: 0,
          created_at: "2024-06-06",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
