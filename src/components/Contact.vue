<template>
	<div >
	<div class="contactme">
	
		<h2 class="title">联系我</h2>
		<div class="info">
			<div class="contactway">
				<div>
					<h3 class="layout">联系方式</h3>
				</div>
				
				<div>
					<span>
					<svg class="icon" >
			    		<use xlink:href="#icon-mao2"></use>
					</svg>
					</span>
					江苏省镇江市
					
				</div>		
				<div>
					<span>
					<svg class="icon" >
			    		<use xlink:href="#icon-dianhua"></use>
					</svg>
					15251833069
				</span>
					
				</div>
				<div>
					<span>
					<svg class="icon" >
			    		<use xlink:href="#icon-qq"></use>
					</svg>
					1240627866	
				</span>
					
				</div>			
				<div>
					<span>
					<svg class="icon" >
			    		<use xlink:href="#icon-youxiang"></use>
					</svg>
					1240627866@qq.com
				</span>
					
				</div>		
				
			</div>
			<div class="message">
			<h3 class="layout">给我留言</h3>
			      
			<input class="layout"
			 style="height:50px; width:188px;border-radius:5px;padding: 10px 10px;"
			placeholder="姓名"
			v-model="input1">
			</input> 
			<input class="layout"
			style="height:50px; width:188px;border-radius:5px;padding: 10px 10px;"
			placeholder="邮箱"
			v-model="input2">
			</input>
			<textarea class="message"
			  style="height:200px; width:400px; border-radius:5px;padding: 10px 10px;"			
			  placeholder="输入内容"
			  v-model="textarea">
			</textarea>

			<button>发送</button>

			</div>
		</div>
	</div>
	</div>

</template>
<script scpoed>
export default {
  data() {
    return {
      textarea: '',
      input1: '',
      input2:''
    }
  }
}
</script>
<style>
	.contactway{
		height: 335px;
		display: flex;
		flex-direction:column;
		justify-content: space-between;
		align-content: center;
		align-items: flex-start;
	}
	.contactway .icon{
		height: 30px;
	}
	.contactme{
		padding:100px 0;
		margin:0 auto;
		width:1280px;
	    color:white;
	}
	.layout{
	 margin:16px 8px;
		
	    
	}
	.title{
		padding:30px auto;
	}
	
	 .info{
	 	display:flex;
	 	justify-content:space-between;
	 }
	 
	 .message {
	 	
	 	width:450px;
	 }
	 .message >button{
	 margin-top:16px;
	 height:50px;
	 width:400px;
	 border-radius:5px;
	 border:2px solid #292929;
	 background:rgb(60,174,162);
	 }
	 .message >button:hover{
	 border:2px solid white;
	 }
</style>