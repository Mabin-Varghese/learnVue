<template>
  <section>
    <div class="container mt-5 pt-5  ">
      <h1>{{ title }}</h1>
      <p>{{ description }}</p>

      <div class="btn d-flex justify-content-center">
        <button @click="onClickBtn" class="btn btn-secondary">Click Here</button>
        <button @click="onClear" class="btn btn-danger ms-2 ">Clear</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      title: '',
      description: ''
    }
  },
  methods: {
    onClickBtn() {
      this.title = 'hello world'
      this.description =
        'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis veritatis, itaque repellat ratione totam ex porro consequatur, recusandae doloremque reiciendis dolores rerum! Dolores rem minus quia, quasi laborum modi sunt?'
    },
    onClear() {
      this.title = ''
      this.description =
        ''
    }
  }
}
</script>
