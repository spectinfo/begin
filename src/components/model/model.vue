<template>
	<main>
		<div>
			<div class="main-right">
				<div class="con-underline">
					<div class="dns-num">
						<span>当前恶意域名数量：</span> <span class="num-class">{{ dnsnum }}</span>
					</div>
				</div>
				<router-view></router-view>
			</div>
			<div id="inp">
		  	<el-input placeholder="请输入网址"  v-model="inputs">
		    	<el-button slot="append" icon="search" @click="onSubmit">确定</el-button>
		  	</el-input>
			</div>
		</div>
	</main>
</template>

<script>
	export default{
		data(){
			return{
				dnsnum:3000
			}
		},
		methods: {
      onSubmit() {
        alert('SECUSS');
      }
    }
	}
</script>

<style>
#inp{
	width: 40%;
	height: 20%;
	margin-left: 30%;
	margin-top: 15%;
}
main{
	border: solid 20px #E9ECF1;
	margin-top: 50px;
	background-color: #FCFCFC;
	min-height: 855px;
	min-width: 1400px;
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	overflow: hidden;
}
.main-right{
	-webkit-box-flex:5.5;
	-ms-flex:5.5;
	flex:5.5;
	padding: 20px 40px;
}
.con-underline{
	border-bottom: 1px solid #CCCCCC;
	height: 40px;
}
.dns-num{
	border-left: 8px solid #72b16a;
}
.dns-num span{
	padding-left: 15px;
	color: #72b16a;
}
.num-class{
	padding-left:5px!important;
	color: orange!important;
}
</style>
