# Ex09 Event Registration Web Application
## Date:15|10|2025

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
```
home.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sports Day - Home</title>
  <link rel="stylesheet" href="home.css">
</head>
<body>
  <div class="phone">
    <img src="logo.png" alt="College Logo" class="logo">
    <h2>SPORTS DAY EVENTS</h2>
    <button class="btn">LOGIN</button>
    <button class="btn">REGISTER</button>
    <div class="footer">“BORN TO WIN”</div>
  </div>
</body>
</html>
home.css
body {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(180deg, #e3f2fd, #fff);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.phone {
  width: 360px;
  height: 700px;
  background: #fff url('home-bg.jpg') no-repeat center/cover;
  border-radius: 35px;
  box-shadow: 0 10px 20px rgba(0,0,0,0.3);
  padding: 30px 20px;
  text-align: center;
  position: relative;
}

.logo {
  width: 120px;
  margin: 0 auto 10px;
  display: block;
}

h2 {
  color: #004aad;
  font-weight: 700;
  margin-bottom: 40px;
  font-size: 20px;
}

.btn {
  display: block;
  width: 80%;
  margin: 15px auto;
  padding: 15px 0;
  border: none;
  border-radius: 25px;
  font-size: 18px;
  cursor: pointer;
  background: #e53935;
  color: white;
  transition: 0.3s;
}

.btn:hover {
  background: #c62828;
}

.footer {
  position: absolute;
  bottom: 20px;
  width: 100%;
  text-align: center;
  font-weight: 600;
  color: #222;
}

events.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sports Day Events</title>
  <link rel="stylesheet" href="events.css">
</head>
<body>
  <div class="phone">
    <h2>SPORTS DAY EVENTS</h2>
    <ul>
      <li>CRICKET</li>
      <li>BADMINTON</li>
      <li>VOLLEY BALL</li>
      <li>100 MTS</li>
      <li>200 MTS</li>
      <li>400 MTS</li>
      <li>4x100 RELAY</li>
    </ul>
  </div>
</body>
</html>

events.css
body {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(180deg, #dfe9f3, #fff);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.phone {
  width: 360px;
  height: 700px;
  border-radius: 35px;
  background: url('events-bg.jpg') no-repeat center/cover;
  box-shadow: 0 10px 20px rgba(0,0,0,0.3);
  color: #000;
  text-align: center;
  padding-top: 60px;
}

h2 {
  color: #d32f2f;
  font-size: 22px;
  margin-bottom: 30px;
}

ul {
  list-style: none;
  padding: 0;
  font-size: 18px;
  font-weight: 500;
  line-height: 2.2em;
}

li::before {
  content: "★ ";
  color: #1565c0;
}

register.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Event Registration</title>
  <link rel="stylesheet" href="register.css">
</head>
<body>
  <div class="phone">
    <h2>EVENT REGISTRATION FORM</h2>
    <form>
      <input type="text" placeholder="Full Name" required>
      <select required>
        <option value="">Gender</option>
        <option>Male</option>
        <option>Female</option>
      </select>
      <input type="number" placeholder="Age" required>
      <input type="text" placeholder="Register Number" required>
      <input type="text" placeholder="Department" required>
      <input type="tel" placeholder="Mobile Number" required>
      <input type="email" placeholder="Email ID" required>
      <input type="text" placeholder="Events to Register" required>
      <button class="btn">REGISTER</button>
    </form>
  </div>
</body>
</html>

register.css
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: linear-gradient(180deg, #f8f9fa, #fff);
}

.phone {
  width: 360px;
  height: 700px;
  border-radius: 35px;
  background: url('register-bg.jpg') no-repeat center/cover;
  box-shadow: 0 10px 20px rgba(0,0,0,0.3);
  padding: 30px 20px;
  color: #000;
}

h2 {
  text-align: center;
  color: #c62828;
  margin-bottom: 20px;
}

input, select {
  width: 100%;
  padding: 12px;
  margin: 8px 0;
  border-radius: 8px;
  border: 1px solid #999;
  font-size: 15px;
}

.btn {
  width: 100%;
  background: #e53935;
  color: #fff;
  border: none;
  padding: 14px;
  border-radius: 25px;
  font-size: 17px;
  margin-top: 10px;
  cursor: pointer;
  transition: 0.3s;
}

.btn:hover {
  background: #b71c1c;
}

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Thank You</title>
  <link rel="stylesheet" href="contact.css">
</head>
<body>
  <div class="phone">
    <img src="logo.png" alt="College Logo" class="logo">
    <h2>THANK YOU</h2>
    <p>We are all eagerly waiting for your participation in the sports events!</p>
    <div class="contact">
      <span>Contact us</span><br>
      Email: saveethaengineeringcollege@gmail.com<br>
      Phone: 6369 643 394 / 6369 643 494
    </div>
  </div>
</body>
</html>

contact.css
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: linear-gradient(180deg, #e3f2fd, #fff);
}

.phone {
  width: 360px;
  height: 700px;
  border-radius: 35px;
  background: url('contact-bg.jpg') no-repeat center/cover;
  box-shadow: 0 10px 20px rgba(0,0,0,0.3);
  padding: 40px 20px;
  text-align: center;
  color: #000;
}

.logo {
  width: 100px;
  margin-bottom: 15px;
}

h2 {
  color: #004aad;
  margin-bottom: 20px;
}

p {
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 40px;
}

.contact {
  font-size: 14px;
  line-height: 1.6em;
}

.contact span {
  color: #2e7d32;
  font-weight: 600;
}
```

## OUTPUT:
![WhatsApp Image 2025-10-15 at 22 32 06_e40d6aa5](https://github.com/user-attachments/assets/2d1aeef6-5d8a-4619-b481-cf421fc99614)
![WhatsApp Image 2025-10-15 at 22 32 06_39ba43c7](https://github.com/user-attachments/assets/94093981-e7ad-42fc-a79b-cc62968cb82d)
![WhatsApp Image 2025-10-15 at 22 32 07_a38c8c1a](https://github.com/user-attachments/assets/c168e168-5f8c-4787-adf1-6ee32a8c7865)
![WhatsApp Image 2025-10-15 at 22 32 07_b4529670](https://github.com/user-attachments/assets/38489297-89b0-4773-a17d-cbb9c50936b6)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
