<?php
// Set the correct password here
$correct_password = "19299182p"; 

// Time limit for lock-out in seconds
$lockout_duration = 3600; 

// Initialize the lock-out data (you might want to store this in a database)
$lockout_ips = [];


function handleData($password, $ip) {
  global $correct_password, $lockout_duration, $lockout_ips;

  // Check if the IP is currently locked out
  if (isset($lockout_ips[$ip]) && $lockout_ips[$ip] > time()) {
    echo "lock_out";
    return;
  }

  // Check if the provided password is correct
  if ($password !== $correct_password) {
    // Increase the number of failed attempts for this IP
    if (!isset($lockout_ips[$ip])) {
      $lockout_ips[$ip] = 0;
    }
    $lockout_ips[$ip]++;

    // Check if the number of failed attempts exceeds the limit
    if ($lockout_ips[$ip] >= 3) {
      // Lock out the IP for the specified duration
      $lockout_ips[$ip] = time() + $lockout_duration;
      echo "lock_out";
      return;
    }

    echo "Key_incorrect";
    return;
  }

  // If the password is correct, reset the failed attempt counter
  $lockout_ips[$ip] = 0;

  


  // File path to store the data
  $dataFile = 'data.txt'; 

  
  if (isset($_POST['data'])) {
    file_put_contents($dataFile, $_POST['data']);
    echo "Ok";
  } else {
    // Read the data from the file
    $data = file_get_contents($dataFile);
    if ($data) {
      echo $data;
    } else {
      echo "no_data";
  }
}
}
$ip = $_SERVER['REMOTE_ADDR'];
$password = isset($_POST['password']) ? $_POST['password'] : null;
handleData($password, $ip);
?>
