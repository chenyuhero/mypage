<template>
	<div >
	<div id="navbar">
		<div class="navheader">我</div>
		<div class="navlist">
			<ul>
				<li>主页</li>
				<li>关于</li>
				<li>作品</li>
				<li>联系</li>
			</ul>
		</div>
	</div>
	</div>	
</template>

<style >
#navbar{
	width: 100%;
	display: flex;
	justify-content: space-around;
	color:white;
}
.navheader{
 float:left;
 margin:20px 0;
 font-size:24px;
}
.navlist{
float:right;
}
.navlist>ul>li{
display:inline-block;
margin:25px 20px;
font-size:16px;
}
	
.navlist>ul>li:hover{
	cursor:pointer;
}	
	

</style>