<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>微信消息</title>
		<style type="text/css">
		/* 	#d1{
				width: 200px;
				height: 200px;
				background: pink;
				border-top:20px solid orangered;
				border-bottom:20px solid blue;
				border-left:20px solid yellow;
				border-right:20px solid cyan;
				
			} */
			.liaotian{
				width: 500px;
				line-height: 100px;
				background: lawngreen;
				padding: 50px;
				font-size: 30px;
				margin: 200px;
				border-radius: 30px;
				position: relative; /*子元素 相对定位 */
			}
			.liaotian:before{
				content:""; /* "微信聊天框"字段前面的内容 */
				display: inline-block; /* 为了设置成行块 */
				width: 0px;
				height: 0px;
				background: transparent;
				border-top: 40px solid transparent;
				border-bottom: 40px solid transparent;
				border-left: 40px solid transparent;
				border-right: 40px solid lawngreen;
				position: absolute; /* 伪元素绝对定位 */
				left: -80px;
				top: 60px;
			}
			.chat:after{
				/* content:"after的内容" */
				content: "";
			}
		</style>
	</head>
	<body>
		<div id="d1"></div>
		<p></p>
	
		<div class="liaotian">
			珺珺快睡觉
			
		</div>
	</body>
</html>
