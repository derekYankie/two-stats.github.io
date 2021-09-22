<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Two Stats</title>
</head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<style type="text/css">


</style>

<body>

  <h1> You have two stats...</h1>

<input type="button" value="click for stats" id="shuffle">

<ul class="mylist">
 <li id="id1">Power</li>
 <li id="id2">Silliness</li>
 <li id="id3">Reality</li>
 <li id="id4">Unreality</li>
 <li id="id5">Adventure</li>
 <li id="id6">Horror</li>
 <li id="id7">Apprehension</li>
 <li id="id8">Annoyance</li>
 <li id="id9">Philosophy</li>
 <li id="id10">Infatuation</li>
 <li id="id11">Annoyance</li>
 <li id="id12">Despair</li>
</ul>



</body>

<script type="text/javascript">

$(document).ready(function(){
	$("ul.mylist li").slice(2).hide();

	var theCount  = 2;
	$("#shuffle").click(function(){
		
		$("ul.mylist li").hide();

		var theLength = $("ul.mylist li").length;
		if(theCount == theLength)
		{
			theCount = 2;
		}
		else
		{
			theCount = theCount + 3;
		}

		$("ul.mylist li").slice(theCount-2,theCount).show();
		
	 });	
	});
</script>

</html>


