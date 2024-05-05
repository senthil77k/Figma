# Ex09 Event Registration Web Application
## Date:
06.05.2024

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
page 1:
```
HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Saveetha Engineering College Sports Day</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="header-content">
      <h1>SAVEETHA ENGINEERING COLLEGE</h1>
      <p>Autonomous  TNEA CODE 1216</p>
      <p>AAICTE Affliated Asi˹..˺</p>
    </div>
  </header>
  <main>
    <div class="main-content">
      <h2>SPORTS DAY</h2>
      <div class="register-login">
        <a href="#">REGISTER</a>
        <a href="#">LOGIN</a>
      </div>
    </div>
  </main>
</body>
</html>

CSS

body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}

header {
  background-color: #003399;
  color: #fff;
  padding: 20px;
}

.header-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  font-size: 2em;
  margin-bottom: 10px;
}

p {
  font-size: 0.8em;
  margin-bottom: 5px;
}

main {
  padding: 40px;
}

.main-content {
  text-align: center;
}

h2 {
  font-size: 1.5em;
  margin-bottom: 20px;
}

.register-login {
  display: flex;
  justify-content: space-between;
  width: 200px;
  margin: 0 auto;
}

a {
  color: #003399;
  text-decoration: none;
  font-size: 1em;
  padding: 10px 20px;
  border: 1px solid #003399;
  border-radius: 5px;
}

a:hover {
  background-color: #003399;
  color: #fff;
}
```
PAGE 2:
```
HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Events</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="header-content">
      <h1>EVENTS</h1>
    </div>
  </header>
  <main>
    <div class="event-list">
      <ul>
        <li>Cricket</li>
        <li>Tennis</li>
        <li>Volleyball</li>
        <li>Table Tennis</li>
        <li>Baseball</li>
        <li>Field Hockey</li>
      </ul>
    </div>
  </main>
</body>
</html>

CSS

body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}

header {
  background-color: #2980b9;
  color: #fff;
  padding: 20px;
  text-align: center;
}

.header-content {
  display: flex;
  justify-content: center;
  align-items: center;
}

h1 {
  font-size: 2em;
  margin-bottom: 0;
}

main {
  padding: 40px;
}

.event-list {
  list-style: none;
  padding: 0;
  margin: 0;
  text-align: center;
}

li {
  font-size: 1.2em;
  margin-bottom: 10px;
}

```
PAGE 3:
```
HTML

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Event Registration Form</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="header-content">
      <img src="soccer_ball.jpg" alt="Soccer Ball">
      <h1>EVENTS FORM</h1>
    </div>
  </header>
  <main>
    <div class="registration-form">
      <form action="/action_page.php" method="post">
        <div class="form-group">
          <label for="name">NAME:</label>
          <input type="text" id="name" name="name" placeholder="Your Name">
        </div>
        <div class="form-group">
          <label for="gender">GENDER:</label>
          <select id="gender" name="gender">
            <option value="male">Male</option>
            <option value="female">Female</option>
          </select>
        </div>
        <div class="form-group">
          <label for="age">AGE:</label>
          <input type="number" id="age" name="age" placeholder="Your Age">
        </div>
        <div class="form-group">
          <label for="regno">REG.NO:</label>
          <input type="text" id="regno" name="regno" placeholder="Registration Number">
        </div>
        <div class="form-group">
          <label for="sport">SPORT NAME:</label>
          <select id="sport" name="sport">
            <option value="cricket">Cricket</option>
            <option value="hockey">Hockey</option>
            <option value="tennis">Tennis</option>
            <option value="volleyball">Volleyball</option>
            <option value="tabletennis">Table Tennis</option>
            <option value="baseball">Baseball</option>
          </select>
        </div>
        <div class="form-group">
          <label for="branch">BRANCH & DEPT:</label>
          <input type="text" id="branch" name="branch" placeholder="Branch & Department">
        </div>
        <div class="form-group">
          <button type="submit">REGISTER</button>
        </div>
      </form>
    </div>
  </main>
</body>
</html>

CSS

body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}

header {
  background-color: #2980b9;
  color: #fff;
  padding: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.header-content {
  display: flex;
  align-items: center;
}

header img {
  width: 100px;
  margin-right: 20px;
}

h1 {
  font-size: 2em;
  margin-bottom: 0;
}

main {
  padding: 40px;
}

.registration-form {
  width: 400px;
  margin: 0 auto;
  background-color: #fff;
  border: 1px solid #ccc;
  padding: 20px;
  border-radius: 5px;
}

.form-group {
  margin-bottom: 15px;
}

label {
  display: block;
  margin-bottom: 5px;
}

input,
select {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
}

button {
  background-color: #2980b9;
  color: #fff;
  padding: 10px 
}
```
PAGE 4:
```
HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Thank You Card</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="card">
    <h1>SAVEETHA ENGINEERING COLLEGE</h1>
    <p>Thank You!</p>
  </div>
</body>
</html>

CSS

body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
  background-color: #2980b9;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.card {
  background-color: #fff;
  padding: 50px;
  text-align: center;
  border-radius: 10px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
}

h1 {
  font-size: 2em;
  margin-bottom: 20px;
}

p {
  font-size: 1.5em;
}

```
## OUTPUT:
![alt text](<Screenshot 2024-05-06 000849.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
