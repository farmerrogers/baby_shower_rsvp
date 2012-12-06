<?php
  
	
	
	//int he line below, insert: 'MySQL url', 'username', 'password', 'database name'
	$dbc = mysqli_connect ('', '', '', '')  
		or die('Error 19 connecting to MySQL server.');	 

	$your_name = mysqli_real_escape_string($dbc, trim($_POST['yourname']));
	$coming_or_not = mysqli_real_escape_string($dbc, trim($_POST['comingornot']));
	$head_count = mysqli_real_escape_string($dbc, trim($_POST['headcount']));
	$comments = mysqli_real_escape_string($dbc, trim($_POST['comments']));
	 
	$query = "INSERT INTO rsvp_form (your_name, coming_or_not, head_count, comments) " .
		"VALUES ('$your_name', '$coming_or_not', '$head_count', '$comments')";

	$result = mysqli_query($dbc, $query)
		or die('Error 31 querying database.');

		 
	echo 'Thanks, ' . $your_name . '!<br />';
	echo 'You ' . $coming_or_not . ' get to come, <br />';
	echo 'If you added something, expect to hear back soon. <br />'; 
		 
	mysqli_close($dbc);
  


  
  
?>