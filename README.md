$fileName = 'get_flag'; $file = fopen($fileName, "r") or die("Unable to open file!"); $content = fread($file,filesize($fileName)); print($content); fclose($myfile);
 
