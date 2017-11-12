<template>
	<div >
	<div id="navbar1">
		<div class="navheader ">
			<svg class="icon" >
		    		<use xlink:href="#icon-home"></use>
				</svg></div>
		<div class="navlist">
			<ul>
				<li v-on:click="gotop">主页</li>
				<li v-on:click="goAbout">关于</li>
				<li v-on:click="goWork">作品</li>
				<li v-on:click="goContanct">联系</li>
			</ul>
		</div>
	</div>
	</div>	
</template>

<script type="text/javascript">
	export default{
		 methods:{
    		gotop :function(){
      			
     			document.documentElement.scrollTop = 0
    		},    		
    		goAbout:function(){
    			document.documentElement.scrollTop = 600
    		},
    		goWork:function(){
    			document.documentElement.scrollTop = 1038
    		},
    		goContanct:function(){
    			document.documentElement.scrollTop = 5750
    		}


 		 }
}
</script>
<style lang = "scss" >


#navbar1{
display: flex;
justify-content: space-around;
color:white;
	.navheader{
		 float:left;
		 margin:20px 0;
		 font-size:24px;
		 .icon{
		 	fill: #ddd;
		 	height: 25px;
		 }
	}
	.navlist{
		float:right;
		&>ul>li{
			display:inline-block;
			margin:25px 20px;
			font-size:16px;
		}
	
		&>ul>li:hover{
			cursor:pointer;
		}	
	}

}



</style>