# subject-220711

```javascript
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.0.1/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

<script>
var str = "こんにちは世界";
// 0:こ, 1:ん, 2:に, 3:ち, 4:は, 5:世

$(function(){

	$("#btn").on("click",function(){
		console.log(  str.indexOf( "世界" )  );
		console.log(  str.indexOf( "日本" )  );

		$("<h6 class='alert alert-secondary'>")
			.appendTo($("#m1"))
			.addClass("mt-3")
			.text( str.indexOf( "世界" ) + " : " + str.indexOf( "日本" ) )
			;
	});

});
</script>
<h5 class="alert alert-primary">サンプル</h5>
<div id="content" class="m-4">
	<div id="m1">
		<input id="btn" name="btn" type="button" value="実行" class="btn btn-primary">
	</div>
</div>
```
