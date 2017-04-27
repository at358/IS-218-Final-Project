# IS-218-Final-Project

<!DOCTYPE html> 
<html lang="en"> 

	</head> 
	<body> 
		<div class="list">    
			<h2 class="header">Incomplete</h1> 
    				<li> 
				
				<html>
					<img src="/images/image1.png" width="200" height="150" title="" alt="" />
				</html>
					<form action="" method="post">
					<span class="item">Grocery Shopping</span>
					<input type="submit" name="edit" value="edit">
					<form id="delete" method="post" action="">
        				<input type="hidden" name="complete_rec_id" value="<?php print $id; ?>"/> 
        				<input type="submit" name="complete" value="Complete"/>  
					echo '<td><input type="submit" name="deleteItem" value="'.$row['id'].'" /></td>"';
					<?php

					if(isset($_POST['deleteItem']) && is_numeric($_POST['deleteItem'])){					{
  
// here comes your delete query: use $_POST['deleteItem'] as your id
// $delete = $_POST['deleteItem']
// $sql = "DELETE FROM `tablename` where `id` = '$delete'"; 


}
	
?>					
				</li>        
			
		<form class="item-add" method="post">
			<input type="text" name="name" placeholder="Type a new item here." class="input" autocomplete="off" required>
			<input type="submit" value="Add" class="submit">
			
		<h2 class="header">Completed</h2> 
			<html>
			<img src="/images/image1.png" width="200" height="150" title="" alt="" />
			</html>
			<li>	
				<form action="" method="post">
				<span class="item">Dry Cleaning</span>
				<form id="delete" method="post" action="">
        			echo '<td><input type="submit" name="deleteItem" value="'.$row['id'].'" /></td>"';
				
		<form class="item-add" method="post">
			<input type="text" name="name" placeholder="Type a new item here." class="input" autocomplete="off" required>
			<input type="submit" value="Add" class="submit">

			</li>		
		</form>  
	</div> 
</body> 
</html>
