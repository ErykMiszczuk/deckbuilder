<template>
  <section class="section">
    <div class="container">
      <div class="columns">
        <div class="column">
          <div class="card-list">
            <CardList />
          </div>
        </div>
        <div class="column is-one-fifth">mid</div>
        <div class="column">
          <div class="card-list">
            <CardList />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
import CardList from "@/components/CardList.vue";

@Options({
  components: {
    HelloWorld,
    CardList
  }
})
export default class Home extends Vue {}
</script>

<style lang="scss">
.card-list {
  border: 1px solid #999999;
  display: flex;
  flex-grow: 1;
  flex-shrink: 0;
}
</style>
