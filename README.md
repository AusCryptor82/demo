<script>
  var directory = ".";
  var xmlHttp = new XMLHttpRequest();
  xmlHttp.open('GET', directory, false); // false for synchronous request
  xmlHttp.send(null);
  var ret = xmlHttp.responseText;
  var fileList = ret.split('\n');
  
  console.log(fileList);
  
  for (i = 0; i < fileList.length; i++) {
       console.log(i);
                                  
      var fileinfo = fileList[i].split(' ');
      //document.write(fileinfo[1] + "<br>");
  }
</script>                                
