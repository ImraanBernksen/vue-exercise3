<template>
<div class="contact_form">
  <form action="/action_page.php">
    <label for="fname">First Name</label>
    <input type="text" id="fname" name="firstname" placeholder="First name">

    <label for="lname">Last Name</label>
    <input type="text" id="lname" name="lastname" placeholder="Last name">

    <label for="lname">Phone Number</label>
    <input type="number" id="lname" name="number" placeholder="Phone number">

    <label for="lname">Email</label>
    <input type="email" id="lname" name="email" placeholder="name@example.com">
  
    <input type="submit" value="Submit">
  </form>
</div>

</template>
<script>
export default {
    name: 'ContactForm'
}
</script>
<style>
input[type=text], input[type=number],input[type=email] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

input[type=submit] {
  width: 100%;
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
}

.contact_form {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}
</style>