<template>
  <div class="contact">
    <div class="contact-buttons">
      <div class="linked-in">
        <h1>Add me on LinkedIn:</h1>
        <a
          href="https://www.linkedin.com/in/jackieodonnell/"
          target="_blank"
          id="linkedin-btn"
          >Connect</a
        >
      </div>
      <div class="resume">
        <h1>Download my resume:</h1>
        <a
          href="/Jackie_Odonnell_Resume.pdf"
          download="Jackie_Odonnell_Resume"
          id="resume-btn"
          >Download</a
        >
      </div>
    </div>
    <div class="email-form">
      <h1>Shoot me an email:</h1>
      <form
        action="mailto:jodonnell287@gmail.com"
        method="POST"
        enctype="text/plain"
        name="EmailForm"
      >
        <label for="name">Name:</label><br />
        <input type="text" name="name" id="name" /><br />
        <label for="email">Email:</label><br />
        <input type="text" name="email" id="email" /><br />
        <label for="ContactComment">Message:</label><br />
        <textarea
          name="ContactComment"
          id="ContactComment"
          cols="30"
          rows="10"
        ></textarea
        ><br />
        <button id="submit-form-btn">Submit</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "contact",
};
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
  width: 50%;
  min-width: 340px;
  display: flex;
  justify-content: space-around;
  margin-top: 5%;
  margin-left: auto;
  margin-right: auto;
}

#linkedin-btn,
#resume-btn {
  background-color: #ecebebec;
  padding: 8px;
  padding-inline: 20px;
  width: 120px;
  font-family: "Poppins-Regular";
  text-transform: uppercase;
  font-weight: 700;
  border-radius: 8px;
  border: none;
  box-shadow: 13px 4px 22px 3px rgba(30, 29, 29, 0.739);
  transition: all 0.2s ease-in-out;
  text-decoration: none;
  color: #e25250;
}

#linkedin-btn:hover,
#resume-btn:hover {
  color: #ecebeb;
  background-color: #e25250;
  box-shadow: 13px 4px 22px 3px rgba(30, 29, 29, 0.875);
  transform: scale(1.05);
}

.email-form {
  display: flex;
  flex-direction: column;
  margin-top: 5%;
  color: #ecebeb;
  font-family: "Poppins-Regular";
  text-transform: lowercase;
  width: 60%;
  min-width: 370px;
  margin-left: auto;
  margin-right: auto;
}

.email-form form {
  background-color: #ecebebec;
  border-radius: 8px;
  box-shadow: 13px 4px 22px 3px rgba(30, 29, 29, 0.875);
  padding: 10px;
  align-self: center;
  min-width: 80%;
  margin-bottom: 100px;
}

.email-form label {
  font-size: 1.2rem;
  color: #313030;
  font-family: "Poppins-Regular";
}

.email-form input {
  width: 90%;
  height: 30px;
  padding-left: 5px;
  background-color: #ecebebe3;
  border: 0.03px solid gray;
  border-radius: 3px;
  box-shadow: 13px 4px 22px 3px rgba(142, 136, 136, 0.285);
  margin-top: 5px;
  margin-bottom: 10px;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 1rem;
}

.email-form textarea {
  padding-top: 5px;
  padding-left: 5px;
  background-color: #ecebebe3;
  border: 0.03px solid gray;
  border-radius: 3px;
  box-shadow: 13px 4px 22px 3px rgba(142, 136, 136, 0.285);
  margin-top: 5px;
  margin-bottom: 10px;
  font-family: Arial, Helvetica, sans-serif;
  width: 90%;
  font-size: 1rem;
}

.email-form button {
  background-color: #519cba;
  padding: 10px;
  padding-inline: 20px;
  margin-bottom: 20px;
  font-family: "Poppins-Regular";
  text-transform: uppercase;
  font-weight: 700;
  font-size: 1rem;
  border-radius: 8px;
  border: none;
  box-shadow: 3px 4px 22px 3px rgba(30, 29, 29, 0.293);
  transition: all 0.2s ease-in-out;
  text-decoration: none;
  color: #ecebeb;
}

.email-form button:hover {
  box-shadow: 3px 4px 22px 3px rgba(30, 29, 29, 0.314);
  transform: scale(1.01);
  background-color: #4691ae;
}
</style>
