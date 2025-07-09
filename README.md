# Saveetha_Admission_clone
## Date:9/7/2025

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saveetha</title>
    <link rel="stylesheet" href="color.css">
</head>
<body>
    <section class="container">
        <div class="left">
            <h1>Saveetha Engineering College</h1>
        </div>
        <div class="right">
     <form class="enquiry-form">
        <h2>Admission Enquiry</h2>
        <label for="name">Full Name</label>
        <input type="text" id="name" placeholder="name" required />
        <label for="email">Email</label>
        <input type="email" id="email" placeholder="mail@example.com" required />
        <label for="phone">Phone Number</label>
        <input type="tel" id="phone" placeholder="9876543210" required />
        <label for="city">City</label>
        <input type="text" id="city" placeholder="city" required />
        <label for="state">State</label>
        <input type="text" id="state" placeholder="state" required />
        <label for="course">Course</label>
        <select id="course" required>
          <option value="">Select Course</option>
          <option>B.Tech</option>
          <option>B.E</option>
          <option>M.Tech</option>
        </select>
        <label for="specialization">Specialization</label>
        <input type="text" id="specialization" placeholder="ex: cse,it,etc..." required />
        <button type="submit">APPLY NOW</button>
      </form>
        </div>
    </section>
</body>
</html>
```

## CSS Code:
```
.left{
  flex: 1;
  background: url('./sec-photo.png') no-repeat center center;
  background-size: contain; 
  background-color: grey;
  height: 100vh; 
}
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}
.container{
    display:flex;
    min-height:100vh;
}
.left h1{
    font-size: 32px;
    padding: 10%;
    color: black;
    font-weight: bold;
    font-family: Arial, Helvetica, sans-serif;
}
.right{
  flex: 1;
  background-color: grey;
  padding: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.enquiry-form{
  width: 100%;
  max-width: 450px;
  padding: 20px;
  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 10px;
}
.enquiry-form h2{
  margin-bottom: 20px;
  color: #005baa;
}
.enquiry-form label{
  display: block;
  margin-top: 15px;
  margin-bottom: 5px;
  font-weight: bold;
}
.enquiry-form input,
.enquiry-form select{
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 6px;
}
.enquiry-form button{
  margin-top: 20px;
  padding: 12px;
  width: 100%;
  background-color: #005baa;
  color: #ffffff;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-size: 16px;
  transition: background 0.3s;
}
.enquiry-form button:hover{
  background-color: #004080;
}
@media(max-width: 768px) {
  .container {
    flex-direction: column;
  }
  .left, .right{
    width: 100%;
    flex:none;
    padding: 20px;
  }
}
.left{
    text-align: center;
}
```

## Output:
![image](https://github.com/user-attachments/assets/88a81b16-0aae-407e-b02f-2aa02ab05fcc)

## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
