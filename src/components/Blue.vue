<template>
  <div>
    <p>This is {{ blueTitle }} title!</p>
  </div>
</template>

<script>
export default {
  data () {
    return {
      blueTitle: 'blue'
    }
  }
}
</script>

<style scoped>
div{
	border: 1px solid #666;
	font-size: 24px;
	color: #fff;
	font-weight: bold;
	text-align: center;
	box-shadow: 1px 1px 2px #333;
	padding: 30px;
	margin: auto;
	background-color: blue;
}
</style>
