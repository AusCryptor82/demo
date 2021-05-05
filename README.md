</div>
</code>

<did id='demo'>
    
</div>    

<script>
 var xmlhttp = new XMLHttpRequest();   
 xmlhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
       document.getElementById("demo").innerHTML = this.responseText;
    }
};
xmlhttp.open("GET", "../index.php", true);
xmlhttp.send();   
    
</script>    
