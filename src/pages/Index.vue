<template>
<Layout>
<h1>Welcome to LifeIQ</h1>
<h2>Augment Your Intelligence</h2>
<button class="button">Learn More</button>
</Layout>
</template>

<script>
import InputWidget from './../components/InputWidget';
import VButton from './../components/VButton';
import InputOperation from './../components/InputOperation';

export default {
  components: {
    InputWidget,
    VButton,
    InputOperation
  },
  data: function () {
    return {
      operator: ''

    }
  },
  methods: {
    onClickInputOperation(value) {
      console.log(value)
    },
    logProps() {
      console.log(InputOperation.props)
    }
  }
}
</script>

<style>
.result {
  border-color: #FFAB00;
}

.grid-container-2 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-auto-rows: 1;
  margin: .5em;
}

.operation-confirm {
  display: flex;
  padding: 0.25em 1em;
  margin: 0 1em 1em 1em;
  background: rgba(50, 75, 125, 0.75);
}
</style>
