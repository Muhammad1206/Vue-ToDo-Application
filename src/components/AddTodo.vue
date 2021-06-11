<template>
  <form @submit.prevent="onSubmit">
    <input type="text" v-model="title" id="input" />
    <button type="submit" class="create-btn">Create</button>
  </form>
</template>

<script>
export default {
  methods: {
    onSubmit() {
      if (this.title.trim()) {
        const newTodo = {
          id: Date.now(),
          title: this.title,
          completed: false,
        };
        this.$emit("add-todo", newTodo);
        this.title = "";
        document.getElementById("input").focus();
      }
    },
  },
  data() {
    return {
      title: "",
    };
  },
};
</script>

<style scoped>
form {
  display: flex;
  justify-content: center;
}
input {
  display: block;
  width: 50%;
  height: 30px;
  border: 1px solid rgb(0, 0, 0);
  outline: none;
  padding: 0px 3%;
}
.create-btn {
  box-shadow:inset 0px 1px 0px 0px #54a3f7;
	background:linear-gradient(to bottom, #007dc1 5%, #0061a7 100%);
	background-color:#007dc1;
	border-radius:3px;
	border:1px solid #124d77;
	display:inline-block;
	cursor:pointer;
	color:#ffffff;
	font-family:Arial;
	font-size:13px;
	padding:6px 24px;
	text-decoration:none;
	text-shadow:0px 1px 0px #154682;
}
</style>
