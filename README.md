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

