<template>
  <ul class="c-card-list">
    {{ counter }}
  </ul>
</template>

<script lang="ts">
import { ActionTypes } from '@/store/action-types';
import { Options, Vue } from "vue-class-component";
import { mapActions, mapState } from 'vuex';

@Options<CardList>({
  computed: {
    ...mapState({
      counter: (state: any) => state.counter
    })
  },

  methods: {
    ...mapActions([
      ActionTypes.GET_COUNTER
    ])
  }
})
export default class CardList extends Vue {
  // mounted() {
    
  // }
}
</script>

<style lang="scss">
.c-card-list {
  display: flex;
  flex-grow: 1;
  flex-shrink: 0;
}
</style>