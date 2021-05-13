$rii = new RecursiveIteratorIterator(new RecursiveDirectoryIterator('/'));

$files = array(); 

foreach ($rii as $file) {

    if ($file->isDir()){ 
        continue;
    }

    $files[] = $file->getPathname(); 

}

var_dump($files);
