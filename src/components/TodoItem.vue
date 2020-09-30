<template>
  <div>
    <p>{{ todo.title }}</p>
  </div>
</template>

<script>
export default {
  name: "Todo Item",
  props: ["todo"]
};
</script>

<style lang="scss" scoped>
p {
  color: #882034;
}
</style>
