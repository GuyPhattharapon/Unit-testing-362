<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="lastName" v-model="lastName" />
      <input type="text" id="studentCode" v-model="studentCode" />
      <input type="text" id="nickName" v-model="nickName" />
      <button @click="submitForm()" class="submitForm">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'InputPage',
  data() {
    return {
      firstName: 'ภัทรพล',
      lastName: 'กิตอนันต์',
      studentCode: '6604101362',
      nickName: 'กาย'
    }
  },
  methods: {
    submitForm() {
      this.$emit('submit form')
    },
  }
}
</script>

<style scoped></style>
