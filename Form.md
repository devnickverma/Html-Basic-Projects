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


#### Type `radio`
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

