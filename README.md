# IS-218-Final-Project

<?php
    $first_name = $_GET['first_name'];
    $last_name = $_GET['last_name'];
    $email = $_GET['email address'];
    $Phone_Number = $_GET['phone_number'];
    $Birthday = $_GET['birthday'];
    $Gender = $_GET['What is your gender'];
 ?>
 <!DOCTYPE html>
 <html>
  <head>
  
  <link rel="stylesheet" type="text/css" href="main.css">
  </head>
  <body>
    <h2>Welcome</h2>
    <p>First name: <?php echo  $first_name; ?></p>
    <p>Last name: <?php echo  $last_name; ?></p>
    <p>Email Address: <?php echo $email; ?></p>
    <p>Phone Number: <?php echo $Phone_Number; ?></p>
    <p>Birthday: <?php echo $Birthday; ?></p>
    <p>Gender: <?php echo $Gender; ?></p>
    <a href="SignIn.html">Do you already have an account?</a>
