<template>
  <div>
    <form @submit.prevent="sendSubject">
      <input type="text" v-model="title" />
      <input type="text" v-model="content" />
      <button type="submit">Nuevo Subject</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "FormSubject",
  data() {
    return {
      title: "",
      content: "",
    };
  },
  methods: {
    sendSubject() {
      fetch("http://localhost:5000/api/v1/newsubject", {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({
          title: this.title,
          content: this.content,
          foro:this.foro
        }),
      })
        .then((response) => response.json())
        .then((data) => {
          console.log(data);
        });
    },
  },
};
</script>

<style scoped></style>

