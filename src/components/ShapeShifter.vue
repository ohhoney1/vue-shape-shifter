<template>
	<div id="shape-shifter">
		<canvas class="canvas"></canvas>
	</div>
</template>

<script>
	import ShapeShifter from "../utils/shape-shifter.js"

	export default {
		name: 'vue-shape-shifter',
		props: {
			content: {
				type: String,
				default: 'hello shape-shifter'
			},
			width: {
                type: Number,
                default: 1000
            },
            height: {
                type: Number,
                default: 600
            },
            fontSize: {
                type: Number,
                default: 200
            },
            time: {
                type: Number,
                default: 2000
            }
		},
		mounted () {
            
            ShapeShifter(this.content, this.width, this.height, this.fontSize, this.time);

        }
	}
</script>

<style>
    * {
        padding: 0;
        margin: 0;
    }
    #shape-shifter {
    	width: 100%;
        height: 100%;
        text-align: center;
        line-height: 100%;
        background-color: #69b4ca;
        /*background: -webkit-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: -moz-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: -o-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: -ms-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);*/
    }
</style>