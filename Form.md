# Form

- An HTML form is used to collect user input. The user input is most often sent to a server for processing.
- `<form>` element is used to create an HTML form for user input
- `<input>` element can be displayed in many ways, 
- depending on the type `<input type="text">` attribute(e.g. text, checkbox, radio)
- `<input type="submit">`	Displays a submit button (for submitting the form)
- `<input type="button">`	Displays a clickable button
- attribute `name="var-name"` variable name for submitting page to backend


#### Type text and email
```html
<!DOCTYPE html>
<html>
<body >
<h1>Student Registration Form </h1>
<pre style="font-family:arial;">

<form action="/action_page.php" >
  <label>First Name</label>
  <input type="text" name="fname">
  <label>Last Name</label>
  <input type="text" name="lname">
  <label>Email</label>
  <input type="email" name="email" >
  <input type="submit">
</form>

</pre>
</body>
</html>
```

#### Type `checkbox`
- unique variable name and value `name="fruit1" value="apple"`
- single variable for single value

```html
<!DOCTYPE html>
<html>
<body >
<h1>Student Registration Form </h1>
<pre style="font-family:arial;">
<form action="/action_page.php" >
  <label>Favorite Fruits</label>  
  <input type="checkbox" name="fruit1" value="apple"><label>Apple</label>
  <input type="checkbox" name="fruit2" value="banana"><label>Banana</label>
  <input type="checkbox" name="fruit3" value="mango"><label>Mango</label>
  <input type="checkbox" name="fruit4" value="grapes"><label>Grapes</label>
  <input type="submit">
</form>
</pre>
</body>
</html>
```
- Output
![Capturedfsfd](https://user-images.githubusercontent.com/105803143/169856733-893e87d3-be82-468b-a35b-12c86e8b6565.PNG)




#### Type `radio`
- single variable for many values
- `name="gender"` `value="male"` `value="female"`
```html
<!DOCTYPE html>
<html>
<body >
<h1>Student Registration Form </h1>
<pre style="font-family:arial;">
<form action="/action_page.php" >
  <label>Gender</label>  
  <input type="radio" name="gender" value="male"><label>Male</label>
  <input type="radio" name="gender" value="female"><label>Female</label>
  <input type="radio" name="gender" value="other"><label>Other</label>
  <input type="submit">
</form>
</pre>
</body>
</html>
```
- Output

![form](https://user-images.githubusercontent.com/105803143/169855582-1eea925c-b8da-4f10-8cf2-b3256c2fb9a6.PNG)


#### Submit Button
- `<input type="submit">` defines a button for submitting the form data to a form-handler.
-  form-handler is specified in the form's `action` attribute


#### Name Attribute
- input field must have a name attribute to be submitted


#### Form Task 1
```html

<!DOCTYPE html>
<html>
<body>
<h1>Student Admission Form</h1>
  <form action="/action_page.php">
  <label>First Name:</label><br>
  <input type="text" name="fname" placeholder="Frist Name" ><br>
  <label>Last Name:</label><br>
  <input type="text" name="lname" placeholder="Last Name" ><br>
  <label>Father's Name:</label><br>
  <input type="text" name="fathersname" placeholder="Father's Name" ><br>
  <label>Email:</label><br>
  <input type="email" name="email" placeholder="Email" ><br>
  <label>Phone no. :</label><br>
  <input type="text" name="phoneno." placeholder="Phone no.:" ><br>
<label>Course :</label><br>
  <input type="radio" name="course" value="B.tech/Be" ><label>B.tech/Be</label><br>
  <input type="radio" name="course" value="BSC" ><label>BSC</label><br>
  <input type="radio" name="course" value="B.COM" ><label>B.COM</label><br>
  <input type="radio" name="course" value="BA" ><label>BA</label><br>
  <input type="radio" name="course" value="BCA" ><label>BCA</label><br>
<label>Facility :</label><br>
  <input type="checkbox" name="facility1" value="BUS" ><label>BUS</label><br>
  <input type="checkbox" name="facility2" value="Sport" ><label>Sport</label><br>
  <input type="checkbox" name="facility3" value="Intership" ><label>Intership</label><br>
  <input type="checkbox" name="facility4" value="Special Session" ><label>Special Session</label><br>
<input type="submit">
</form>
</body>
</html>
```

#### Action Attribute
- 

