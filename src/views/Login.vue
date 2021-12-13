<template>
  <b-container fluid>
    <b-row class="my-1">
      <b-col sm="3">
        <label for="email">EMAIL<code></code>:</label>
      </b-col>
      <b-col sm="9">
        <b-form-input id="email"></b-form-input>
      </b-col>
    </b-row>

    <b-row class="my-1">
      <b-col sm="3">
        <label for="email">PASSWORD<code></code>:</label>
      </b-col>
      <b-col sm="9">
        <b-form-input id="email"></b-form-input>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
    name : "Login",
    data() {
      return {
        types: [
          'text',
          'number',
          'email',
          'password',
          'search',
          'url',
          'tel',
          'date',
          'time',
          'range',
          'color'
        ]
      }
    }
}
</script>

<style>

</style>