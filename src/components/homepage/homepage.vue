<!--template>
	<main>
		<div id="inp">

		</div>
	</main>
</template>

<script>
	export default{
		data(){
			return{
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

</style-->
<template>
	<main>
	 <div id="inp">
	  <el-carousel :interval="5000" arrow="always">
	    <el-carousel-item v-for="item in 4">
	      <h3>{{ item }}</h3>
	    </el-carousel-item>
	  </el-carousel>
	</div>
</main>
</template>

<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    line-height: 400px;
    margin: 0;
  }

  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }

  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
</style>
