# Custom Table With Design - 20 May 22

# 1. Employee Table Green
```html
<!DOCTYPE html>
<html>
<head>
<style>
table ,tr ,th ,td{
  border:2px solid #DDD;
  border-collapse: collapse;
  text-align:left;
  padding:4px;    
}
  
tr:nth-child(even){
	background-color:#eaf1dd;
}
  
tr:nth-child(odd){
	background-color:#ffffff;
}
  
th{
  color:white;
  background-color: #9bbb59;
}
  
tr:hover {
  background-color: #D6EEEE;
}
</style>
</head>
<body>
<table style=" width:100%;">
   <tr>
    <th>Id</th>
    <th>Name</th>
    <th>Email</th>
    <th>Key</th>
    <th>Default</th>
   </tr>
   <tr>
    <td>231</td>
    <td>Mary S. Brunson</td>
    <td>MarySBrunson@armyspy.com</td>
    <td>Bonds</td>
    <td>Null</td>
   </tr>
   <tr>
    <td>210</td>
    <td>Jan J. Farmer</td>
    <td>JanJFarmer@dayrep.com</td>
    <td>Stocks</td>
    <td>Null</td>
   </tr>
   <tr>
    <td>256</td>
    <td>Dorothy Lacey</td>
    <td>DorothyTLacey@rhyta.com</td>
    <td>Residencial property</td>
    <td>Null</td>
   </tr>
   <tr>
    <td>211</td>
    <td>Lin D. Wimer</td>
    <td>LinDWimer@jourrapide.com</td>
    <td>Stocks</td>
    <td>Null</td>
   </tr>
</table>
</body>
</html>
```
- Output
![green table](https://user-images.githubusercontent.com/105803143/169572620-796808eb-807d-4ca8-95d9-537ba1339b6c.PNG)


# 2. Employee Table Blue

```html
<!DOCTYPE html>
<html>
<head>
<style>
table ,tr ,th ,td{
    border:2px solid #DDD;
    border-collapse: collapse;    
    text-align:left;
    padding:4px; 
}

tr:nth-child(even){
	background-color:#ffffff;
}

tr:nth-child(odd){
	background-color:#def;
}

th{
	background-color:#7daedf;
}
tr:hover {
	background-color: #D6EEEE;
}

</style>
</head>
<body>

<table style=" width:100%;">
   <tr>
    <th>Field</th>
    <th>Type</th>
    <th>Null</th>
    <th>Investments</th>
   </tr>
   <tr>
    <td>209</td>
    <td>Mary S. Brunson</td>
    <td>MarySBrunson@armyspy.com</td>
    <td>Bonds</td>
   </tr>
   <tr>
    <td>210</td>
    <td>Jan J. Farmer</td>
    <td>JanJFarmer@dayrep.com</td>
    <td>Stocks</td>
   </tr>
   <tr>
    <td>256</td>
    <td>Dorothy Lacey</td>
    <td>DorothyTLacey@rhyta.com</td>
    <td>Residencial property</td>
   </tr>
   <tr>
    <td>211</td>
    <td>Lin D. Wimer</td>
    <td>LinDWimer@jourrapide.com</td>
    <td>Stocks</td>
   </tr>
</table>
</body>
</html>
```
- Ouput
![blue table](https://user-images.githubusercontent.com/105803143/169572598-3185023d-ba7f-4399-a36a-67a33179301b.PNG)

