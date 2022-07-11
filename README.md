# subject-220711

```javascript
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.0.1/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

<script>
$(function(){

	$("#btn").on("click",function(){
		$("#result1")
			.text( $("#target1").val().indexOf( $("#serach1").val() ) + " = \"" + $("#target1").val() + "\".indexOf(\"" + $("#serach1").val() + "\");" );
			;
	});

	$("#btn2").on("click",function(){
		$("#result2")
			.text( $("#target2").val().substr( $("#start2").val(),$("#len2").val() ) + " = \"" + $("#target2").val() + "\".substr(" + $("#start2").val() + "," + $("#len2").val() + ");" );
			;
	});

	$("#btn3").on("click",function(){
		$("#result3")
			.text( $("#target3").val().slice( $("#start3").val() ) + " = \"" + $("#target3").val() + "\".slice(" + $("#start3").val() + ");" );
			;
	});

	$("#btn4").on("click",function(){
		$("#result4")
			.text( "[" + $("#target4").val().split( $("#kugiri").val() ) + "] = \"" + $("#target4").val() + "\".split(\"" + $("#kugiri").val() + "\");" );
			;
	});



});
</script>
<h5 class="alert alert-primary">String メソッド</h5>
<div id="content" class="m-4">
	<div id="m1">
		<input type="text" id="target1" value="こんにちは世界">.<input id="btn" name="btn" type="button" value="indexOf" class="btn btn-primary">.<input type="text" id="serach1" value="世界">
		<h6 id="result1" class='alert alert-secondary mt-2'></h6>
	</div>

	<div id="m2">
		<input type="text" id="target2" value="こんにちは世界">.<input id="btn2" name="btn" type="button" value="substr" class="btn btn-primary">.<input type="text" id="start2" value="0">,<input type="text" id="len2" value="5">
		<h6 id="result2" class='alert alert-secondary mt-2'></h6>
	</div>

	<div id="m3">
		<input type="text" id="target3" value="こんにちは世界">.<input id="btn3" name="btn" type="button" value="slice" class="btn btn-primary">.<input type="text" id="start3" value="-3">
		<h6 id="result3" class='alert alert-secondary mt-2'></h6>
	</div>

	<div id="m4">
		<input type="text" id="target4" value="こん,にちは,世界">.<input id="btn4" name="btn" type="button" value="slice" class="btn btn-primary">.<input type="text" id="kugiri" value=",">
		<h6 id="result4" class='alert alert-secondary mt-2'></h6>
	</div>


</div>
```
