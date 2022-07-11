# subject-220711

```javascript
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.0.1/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

<script>
var wk = "こんにちは世界";
// 0:こ, 1:ん, 2:に, 3:ち, 4:は, 5:世

$(function(){

	$("#btn").on("click",function(){
		$("<h6 class='alert alert-secondary'>")
			.appendTo($("#m1"))
			.addClass("mt-3")
			.text( $("#target1").val().indexOf( $("#serach1").val() ) )
			;
	});

});
</script>
<h5 class="alert alert-primary">サンプル</h5>
<div id="content" class="m-4">
	<div id="m1">
		<input type="text" id="target1" value="こんにちは世界">
		<input id="btn" name="btn" type="button" value="indexOf" class="btn btn-primary">
		<input type="text" id="serach1" value="世界">
	</div>
</div>
```
