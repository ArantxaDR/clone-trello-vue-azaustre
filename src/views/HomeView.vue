<template>
  <div>
    <h3>Mis paneles</h3>
    <div class="boards-collection">
      <input
        type="text"
        placeholder="Añade un nuevo panel"
        v-model="boardName"
        @keyup.enter="add()"
      />
      <board-card
        v-for="(board, index) in boards"
        :key="index"
        :name="board.name"
        :id="board.id"
      >
      </board-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "home-view",
};
</script>
<style lang="scss" scoped>
h3 {
  text-align: left;
  margin: 1.5rem;
}
</style>
