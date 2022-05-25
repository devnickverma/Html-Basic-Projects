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
- Output
![student form](https://user-images.githubusercontent.com/105803143/170073751-11310736-3ff2-4ec4-bf21-9d0843b2245d.PNG)



#### Action  Attribute
- `action` attribute defines the action to be performed when the form is submitted
- form data is sent to a file on the server when the user clicks on the `submit` button

#### Target 
- `target` attribute specifies where to display the response that is received after submitting the form
```bash
_blank	The response is displayed in a new window or tab
_self	The response is displayed in the current window
_parent	The response is displayed in the parent frame
_top	The response is displayed in the full body of the window
framename	The response is displayed in a named iframe
```

#### Method Attribute
- `GET` and `POST`
- method attribute specifies the HTTP method to be used when submitting the form data
- default HTTP method when submitting form data is GET. 
- Always use POST if the form data contains sensitive or personal information


```bash
Notes on GET:

Appends the form data to the URL, in name/value pairs
NEVER use GET to send sensitive data! (the submitted form data is visible in the URL!)
The length of a URL is limited (2048 characters)
Useful for form submissions where a user wants to bookmark the result
GET is good for non-secure data, like query strings in Google
Notes on POST:

Appends the form data inside the body of the HTTP request (the submitted form data is not shown in the URL)
POST has no size limitations, and can be used to send large amounts of data.
Form submissions with POST cannot be bookmarked
```

#### Autocomplete Attribute
- autocomplete attribute specifies whether a form should have autocomplete on or off
- off will hide the suggestion when filling form
`<form action="/action_page.php" autocomplete="off">`

#### novalidate attribute in form
- not check any validation like email formate checking
`<form action="/action_page.php" novalidate>`


#### Form Task 2
```html
<!DOCTYPE html>
<html>
<head>
    <style>
        body{
            font-family:arial;
            font-size:20px;

        }

        input{
            border-radius:5px;
            background-color:#a6a6a6;
            border:1px solid #a6a6a6;
            padding:3px;
        }

        button{
            border-radius:5px;
            background-color:#a6a6a6;
            border:1px solid #a6a6a6;
            font-size:14px;         
            padding:10px 15px;
            font-weight: bold;

        }
    </style>
</head>
<body>

    <h1>HTML Form</h1>

    <form action="/action_page.php" method="post">
        <table>
            <tr>
                <td> <label>First Name:</label> </td>
                <td> <input type="text" name="fname"  ></td>        
            </tr> 
            <tr>
                <td> <label>Last Name:</label> </td>
                <td> <input type="text" name="lname"  ></td>        
            </tr>
            <tr>
                <td> <label>Date of Birth:</label> </td>
                <td> <input type="text" name="dob" ></td>        
            </tr>
            <tr>
                <td> <label>Email id:</label> </td>
                <td>  <input type="email" name="email"  ></td>        
            </tr>
            <tr>
                <td> <label>Mobile Number:</label> </td>
                <td>  <input type="text" name="mobileno"  ></td>        
            </tr>
        </table>
        <br><br>
        <button type="submit">SUBMIT</button>&nbsp;&nbsp;<button type="reset">RESET</button>     
    </form>

</body>
</html>
```
- Output
![form task 2](https://user-images.githubusercontent.com/105803143/170230027-20bcf8b6-bae1-4651-b2f2-3769959945ff.PNG)


#### Select Field In Form
- `<select>` element defines a drop-down list
- `<option>` elements defines an option that can be selected
- By default, the first item in the drop-down list is selected
- `<select name="cars" size="3">` attribute to specify the number of visible values
- `<select  name="cars" multiple>` multiple attribute to allow the user to select more than one value
```html
<form action="/action_page.php">  
  <select  name="cars" multiple>
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="fiat">Fiat</option>
    <option value="audi">Audi</option>
  </select>
  <input type="submit">
</form>
```
- Output
![fdfdf](https://user-images.githubusercontent.com/105803143/170276839-8d3eeb80-3edf-4e1c-a924-78991b7360e6.PNG)


#### `<textarea>` element defines a multi-line input field (a text area)
- The `rows` attribute specifies the visible number of lines in a text area.
- The `cols` attribute specifies the visible width of a text area.

```html
<form action="/action_page.php">
  <textarea name="message" rows="5" cols="23">The cat was playing in the garden.</textarea>
  <br><br>
  <input type="submit">
</form>
```
- Output
![textarea](https://user-images.githubusercontent.com/105803143/170277447-3702fc25-1996-401e-a0d3-93400d718646.PNG)

#### Other Input Type
```html
<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password">
<input type="radio">
<input type="range">
<input type="reset">
<input type="search">
<input type="submit">
<input type="tel">
<input type="text">
<input type="time">
<input type="url">
<input type="week">
```
#### 25 May 22 Task 
- Above list try
- Create this
https://www.iaccessworld.com/wp-content/uploads/edd/2014/11/student-form.png
