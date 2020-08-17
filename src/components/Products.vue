<template>
  <div id="products" class="container">
    <h2 class="mt-5">Our Recent Products</h2>
    <div class="form-inline mt-4">
      <input
        class="form-control"
        type="text"
        placeholder="Search Products"
        v-model="search"
      />
    </div>
    <div class="row mt-5">
      <div
        class="col-md-3 pb-4"
        v-for="(item, index) in filteredItems"
        :key="item.id"
      >
        <div class="card">
          <img class="card-img-top" :src="item.image" alt="Card image cap" />
          <div class="card-body">
            <h5 class="card-title">{{ item.title }}</h5>
            <p class="card-text" style="font-size:14px;">
              {{ item.desc }}
            </p>
            <button
              class="btn btn-outline-danger"
              @click="removeElement(index)"
            >
              Delete
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["items"],
  data() {
    return {
      search: "",
    };
  },
  methods: {
    removeElement: function(index) {
      console.log(this.items.splice(index, 1));
    },
  },
  computed: {
    filteredItems() {
      if (this.search) {
        return this.items.filter((item) => {
          return this.search
            .toLowerCase()
            .split(" ")
            .every((v) => item.title.toLowerCase().includes(v));
        });
      } else {
        return this.items;
      }
    },
  },
};
</script>

<style scoped>
* {
  box-sizing: border-box;
}
h2 {
  border-bottom: 1px solid rgb(161, 179, 179);
  color: darkcyan;
}
img {
  width: 100%;
  height: 200px;
}
</style>
