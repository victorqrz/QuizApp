<template>
  <div class="question-box-container">
    <b-jumbotron>

      <template v-slot:lead>
        {{ currentQuestion.question }}
      </template>

      <hr class="my-4">

      <p>
        List of answers !!
      </p>

      <b-button variant="primary" href="#">Submit</b-button>
      <b-button @click="next" variant="success" href="#">
        Next
      </b-button>

    </b-jumbotron>
  </div>
</template>

<script>
export default {
  props: {
    currentQuestion: {
      type: Object,
      required: true
    },
    next: {
      type: Function
    }
  }
}
</script>

<style>

</style>