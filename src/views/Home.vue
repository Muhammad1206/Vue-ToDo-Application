<template>
  <div class="container">
    <h2>Home Page</h2>
    <p>
      ToDo Aplication - is simple and awesome app to organize your tasks with
      very easy to use interface. ToDo can help you to make list of your tasks
      and also you can set Reminder with specific tasks. It reminds you at you
      specified Time. ... So we made user interface like that so that it can
      give you a quick view on your day timeline.
    </p>
    <router-link to="/todos">Todos</router-link>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Baloo+Tammudu+2:wght@500&display=swap');
.container {
  max-width: 1150px;
  margin: 0px auto;
  padding: 0px 10px;
}
p {
  font-size: 20px;
  font-family: 'Baloo Tammudu 2', cursive;
}
a {
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
