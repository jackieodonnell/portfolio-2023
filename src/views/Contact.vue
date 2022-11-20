<template>
  <div class="contact">
    <div class="contact-buttons">
      <div class="linked-in">
        <h1>Add me on LinkedIn:</h1>
        <a href="https://www.linkedin.com/in/jackieodonnell/" id="linkedin-btn">Connect</a>        
      </div>
      <div class="resume">
        <h1>Download my resume:</h1>
        <a href="/Jacqueline_Odonnell_Resume.pdf" download="Jacqueline_Odonnell_Resume" id="resume-btn">Download</a>        
      </div>

    </div>
    <div class="email-form">
      <h1>Shoot me an email:</h1>
      <form action="mailto:jodonnell287@gmail.com" method="POST" enctype="text/plain" name="EmailForm">
        <label for="name">Name:</label><br>
        <input type="text" name="name" id="name"><br>
        <label for="email">Email:</label><br>
        <input type="text" name="email" id="email"><br>
        <label for="ContactComment">Message:</label><br>
        <textarea name="ContactComment" id="ContactComment" cols="30" rows="10"></textarea><br>
        <input type="submit" value="submit" id="submit-btn">
      </form>
    </div>

  </div>
</template>

<script>
export default {
  name: "contact",
}
</script>

<style scoped>
    .contact h1 {
        color: rgb(224, 222, 222);
        font-family: monospace;
        font-weight: 300;
        font-size: 1.2rem;
        text-transform: lowercase;
    }
    .contact-buttons {
      display: flex;
      justify-content: space-around;
      margin-top: 5%;
      margin-left: 20%;
      margin-right: 20%;
    }

    #linkedin-btn, #resume-btn {
      padding: 5px;
      width: 60%;
      background-color: rgba(41, 39, 39, 0.614);
      border: 1.5px solid rgba(135, 135, 135, 0.539);
      border-radius: 5px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.341);
      text-transform: lowercase;
      font-family: monospace;
      font-size: 1.2rem;
      font-weight: 400;
      color: rgba(243, 187, 83, 0.937);
      transition: all 0.3s ease-in-out;
      text-decoration: none;
    }

    #linkedin-btn:hover, #resume-btn:hover {
      background-color: rgba(124, 123, 123, 0.489);
      font-weight: 800;
      color: #5bbbe1;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.727);
      transition: all 0.3s ease-in-out;
    }

    .email-form {
      display: flex;
      flex-direction: column;
      margin-left: 25%;
      margin-right: 25%;
      margin-top: 5%;
      color: white;
      font-family: monospace;
      text-transform: lowercase;
    }

    .email-form form {
      background-color: rgba(41, 39, 39, 0.614);
      border: 1.5px solid rgba(135, 135, 135, 0.539);
      border-radius: 5px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.341);
      padding: 10px;
    }

    .email-form label {
      font-size: 1rem;
      color: rgb(224, 222, 222);
      font-family: monospace;
    }

    .email-form input {
      width: 90%;
      height: 20px;
      padding-left: 5px;
      background-color: rgba(224, 222, 222, 0.993);
      border: 1.5px solid rgba(0, 0, 0, 0.539);
      border-radius: 3px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.341);
      margin-top: 5px;
      margin-bottom: 10px;
      font-family: Arial, Helvetica, sans-serif;
    }

    .email-form textarea {
      padding-top: 5px;
      padding-left: 5px;
      background-color:  rgba(224, 222, 222, 0.993);
      border: 1.5px solid rgba(17, 17, 17, 0.539);
      border-radius: 3px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.341);
      margin-top: 5px;
      margin-bottom: 10px;
      font-family: Arial, Helvetica, sans-serif;
      width: 90%;
    }

    #submit-btn {
      padding: 5px;
      width: fit-content;
      height: fit-content;
      background-color: rgba(41, 39, 39, 0.614);
      border: 1.5px solid rgba(135, 135, 135, 0.539);
      border-radius: 5px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.341);
      text-transform: lowercase;
      font-family: monospace;
      font-size: 1.2rem;
      font-weight: 400;
      color: rgba(243, 187, 83, 0.937);
      transition: all 0.3s ease-in-out;
    }

    #submit-btn:hover {
    background-color: rgba(124, 123, 123, 0.489);
      font-weight: 800;
      color: #5bbbe1;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.727);
      transition: all 0.3s ease-in-out;
    }

</style>
