<template>
  <div class="header">
    <h1>Test réalisé par {{ Name }} {{ Surname }}</h1>
    <h2>réalisé le {{ DateToday }}</h2>
  </div>
</template>

<script>
export default {
  name: "ProgressBar",
  data() {
    return {
      Name: "CHARNAY-KRUSCHAT",
      Surname: "Eva",
      DateToday: "03/10/2022",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-bottom: 100px;
}
h1,
h2 {
  font-weight: bold;
  width: 100%;
}
</style>
