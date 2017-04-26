# IS-218-Final-Project
<?php require_once("includes/connection.php"); ?>
<?php include_once("includes/form_functions.php"); ?>
<?php
    session_start();
	if(isset($_SESSION['registered'])) {
		redirect_to("index.php");
	}
?>
<!DOCTYPE html">

<?php	
	// START FORM PROCESSING
	if (isset($_POST['register'])) { // Form has been submitted.
		$errors = array();

		// perform validations on the form data
		$required_fields = array('fName','lName','email','phone','birthday',' gender ', 'password');
		$errors = array_merge($errors, check_required_fields($required_fields, $_POST));

		$fields_with_lengths = array('fname' => 30, 'lname' => 30, 'email' => 30,'phone' => 15,,'birthday' => 10, 'gender' => 1,'password' => 30);
		$errors = array_merge($errors, check_max_field_lengths($fields_with_lengths, $_POST));
		
		$email       = trim($_POST['email']);
		$pass        = trim($_POST['pass']);
				
		if (empty($errors) ) {
			// insert row into mySQL table
			$query = "INSERT INTO users (fname, lname, email, phone, birthday, gender, password) 
				VALUES ('{$fname}', '{$lname}','{$email}','{$phone}','{$birthday}','{$gender}','{$password}')";
			$result = mysql_query($query, $connection);
			if ($result) {
				$message = "The user was successfully created.";
				$_SESSION['registered'] = 1;
			} else {
				$message = "The user could not be created.";
				$message .= "<br />" . mysql_error();
			}

