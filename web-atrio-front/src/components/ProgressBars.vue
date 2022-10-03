<template>
  <div v-for="item in progressBars" :key="item.id">
    <div class="bloc-progress-bar">
      <h2 class="bloc-progress-bar__name">{{ item.ProgressBarName }}</h2>
      <div class="bloc-progress-bar__number">
        {{ item.ProgressBarNumber }} %
      </div>
      <div id="bloc-progress-bar__table">
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>

        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
        <div class="bloc-progress-bar__table__five empty"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProgressBars",
  data() {
    return {
      isFirst: false,
      isSecond: false,
      isThird: false,
      isFull: false,
      progressBars: [
        {
          id: 1,
          ProgressBarName: "Initialisation du test technique",
          ProgressBarNumber: "25",
        },
        {
          id: 2,
          ProgressBarName: "Avancement de la phase de développement",
          ProgressBarNumber: "50",
        },
      ],
    };
  },
  methods: {
    showProgress() {},
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bloc-progress-bar {
  display: flex;
  flex-wrap: wrap;
  width: 982px;
  padding: 9px;
  margin: 50px auto;
}

.bloc-progress-bar__name {
  width: 100%;
  text-align: left;
  margin: 1rem 0;
}

.bloc-progress-bar__number {
  margin: 0 1rem;
}

#bloc-progress-bar__table {
  width: 840px;
  background: var(--color-dark);
}
</style>
