# IS-218-Final-Project
<?PHP
require_once("./include/membersite_config.php");
?>
<!DOCTYPE html lang="en">
<head>
      
</head>
<body>

<!-- Form Code Start -->
<fieldset >
<Title>Login</Title>

<input type='hidden' name='submitted' id='submitted' value='1'/>

<div class='short_explanation'>* required fields</div>

<div><span class='error'><?php echo $fgmembersite->GetErrorMessage(); ?></span></div>
<div class='container'>
    <label for='email' >Email Address*:</label><br/>
    <input type='text' name='username' id='username' maxlength="50" /><br/>
    
</div>
<div class='container'>
    <label for='password' >Password*:</label><br/>
    <input type='password' name='password' id='password' maxlength="50" /><br/>

</div>
</div>

<div class='container'>
    <input type='submit' name='Submit' value='Submit' />
</div>
<div class='short_explanation'><a href='reset-pwd-req.php'>Forgot Password?</a></div>
</fieldset>
</form>


