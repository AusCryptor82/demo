<script>
  var directory = ".";
  var xmlHttp = new XMLHttpRequest();
  xmlHttp.open('GET', directory, false); // false for synchronous request
  xmlHttp.send(null);
  var ret = xmlHttp.responseText;
  var fileList = ret.split('\n');
  for (i = 0; i < fileList.length; i++) {
       alert(i);                           
      //var fileinfo = fileList[i].split(' ');
      //document.write(fileinfo[1] + "<br>");
  }
</script>                                
