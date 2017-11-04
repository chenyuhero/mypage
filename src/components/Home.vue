<template>
	<div>
	<div id="home">
		<div class="pic" >
			<div class="type">
			<h1>Stay foolish,stay hungry.</h1>
			
			
			</div>
		</div>
		
	</div>
		
	</div>
</template>

<script>
	export default{
		
		
	}
</script>
<style>
	
	@keyframes type{
    from { width: 0;}
	}
	#home{
	width:1280px;
	color:white;
	display:inline-flex;
    justify-content: space-around;
    align-items: center;
	}
	.pic{
	height:580px;
	width:1280px;
	background:url(https://cdn.dribbble.com/users/31752/screenshots/1613357/computer_desk.png) no-repeat ;
	}
	
	.type{
	text-align:left;
	height:330px;
	width:500px;
	float:right;
	margin-top:150px;
	
	}
	.type h1 {
		font: bold 200% Consolas, Monaco, monospace;
		border-right: .1em solid;
		width: 16.5em; /* fallback */
		width: 30ch; /* # of chars */
		margin: 2em 1em;
		white-space: nowrap;
		overflow: hidden;
		animation: typing 10s steps(30, end), /* # of steps = # of chars */
					blink-caret .5s step-end infinite alternate;
	}
	@keyframes typing { from { width: 0; } }
	@keyframes blink-caret { 50% { border-color: transparent; } }
	
</style>