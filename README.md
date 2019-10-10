# form-login
form login with css and html
file html
<!DOCTYPE html>
<html >
  <head>
    <meta charset="utf-8">
    <title>Insert Form</title>
    <link rel="stylesheet" href="css/master.css">
  </head>
  <body>

      <form class="box" action="/insert" method="post">
      <h1>Login</h1>
      {{csrf_field()}}
      <input type="text" name="Name" placeholder="Userame">
      <input type="text" name="Address" placeholder="Address">
      <input type="text" name="Mobile" placeholder="Mobile Number">
      <input type="submit" name="" placeholder="Login">
    </form>
  </body>
</html>


file css
body{
  margin : 0;
  padding: : 0;
  font-family: sans-serif;
  background: #34495e;
}
.box{
  width: 300px;
  padding: 40px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  background: #191919;
  text-align: center;
}

.box h1{
  color: white
  text-transform:uppercase;
  font-weight: 500;
}

.box input[type = "text"],.box input[type = "password"]{
  border: 0;
  background: none;
  display: block;
  margin: 20px auto;
  text-align: center;
  border: 2px solid #3498db;
  padding: 14px 10px;
  color: white;
  outline: none;
  border-radius: 24px;
  transition: 0.25s
}

.box input[type = "text"]:focus,.box input[type="password"]{
width : 280px;
border-color: #2ecc71;
}

.box input[type = "submit"]{
  border: 0;
  background: none;
  display: block;
  margin: 20px auto;
  text-align: center;
  border: 2px solid #2ecc71;
  padding: 14px 40px;
  color: white;
  outline: none;
  border-radius: 24px;
  transition: 0.25s
  cursor:pointer;
}

.box input[type = "submit"]:hover{
  background: #2ecc71;
}

h1{
   color:white;
}
