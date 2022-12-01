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
        color: #ecebeb;
        font-family: "Poppins-Regular";
        font-weight: 300;
        font-size: 1.2rem;
        text-transform: lowercase;
    }
    .contact-buttons {
      display: flex;
      justify-content: space-around;
      margin-top: 5%;
    }

    #linkedin-btn, #resume-btn {
      padding: 5px;
      width: 60%;
      background-color: #e25250c8;
      border: 1.5px solid rgba(135, 135, 135, 0.539);
      border-radius: 5px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.341);
      text-transform: lowercase;
      font-family: "Poppins-Regular";
      font-size: 1.2rem;
      font-weight: 600;
      color: #ecebeb;
      transition: all 0.3s ease-in-out;
      text-decoration: none;
    }

    #linkedin-btn:hover, #resume-btn:hover {
      background-color: #e25250;
      font-weight: 900;
      color: #ecebeb;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.727);
      transition: all 0.3s ease-in-out;
    }

    .email-form {
      display: flex;
      flex-direction: column;
      margin-top: 5%;
      color: #ecebeb;
      font-family: "Poppins-Regular";
      text-transform: lowercase;  
      width: 100%;

      
    }

    .email-form form {
      background-color:#ecebebe5;
      border: 1.5px solid rgba(135, 135, 135, 0.539);
      border-radius: 5px;
      box-shadow: 1px 4px 12px 6px rgba(0, 0, 0, 0.73);
      padding: 10px;
      align-self: center;
      min-width: 80%;
      
    }

    .email-form label {
      font-size: 1rem;
      color: #313030;
      font-family: "Poppins-Regular";
    }

    .email-form input {
      width: 90%;
      height: 20px;
      padding-left: 5px;
      background-color: rgba(224, 222, 222, 0.993);
      border: 1.5px solid rgba(0, 0, 0, 0.539);
      border-radius: 3px;
      box-shadow: 1px 4px 12px 6px rgba(149, 149, 149, 0.341);
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
      box-shadow: 1px 4px 12px 6px rgba(149, 149, 149, 0.341);
      margin-top: 5px;
      margin-bottom: 10px;
      font-family: Arial, Helvetica, sans-serif;
      width: 90%;
    }

    #submit-btn {
      padding: 5px;
      width: fit-content;
      height: fit-content;
      background-color: #519cbabd;
      border: 1.5px solid rgba(135, 135, 135, 0.539);
      border-radius: 5px;
      box-shadow: 1px 4px 12px 6px rgba(149, 149, 149, 0.341);
      text-transform: lowercase;
      font-family: "Poppins-Regular";
      font-size: 1.2rem;
      font-weight: 600;
      color: #313030;
      transition: all 0.3s ease-in-out;
    }

    #submit-btn:hover {
    background-color: #519cba;
      font-weight: 800;
      box-shadow: 1px 4px 12px 6px rgba(81, 80, 80, 0.244);
      transition: all 0.3s ease-in-out;
    }

</style>
