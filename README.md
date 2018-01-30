# itxzytask7
display: flex; flex-direction: column;可以改变主轴方向，这样就能实现垂直方向元素的排列。
.父元素 选择器:first-child 
圆圈画法circle {
	width: 宽px;
	height: 长px;
	background: red;
	-moz-border-radius: 50px;
	-webkit-border-radius: 50px;
	border-radius: 长或宽的一半px;
}   https://css-tricks.com/examples/ShapesOfCSS/。
音频播放；<div class="x" onclick="playaudio();"><audio src="需要的音频文件路径" controls="controls" preload id="musicmp3" hidden></audio>
然后在html尾部加入<script>
function playaudio(){
    var audio = document.getElementById('musicmp3'); 
        if(audio!==null) {             
            if(audio.paused) {                 
                audio.play();  
            }
            else {
                audio.pause();
            }
        } 
    }
</script>
三角形画法triangle-down {
	width: 0;
	height: 0;
	border-left: 50px solid transparent;
	border-right: 50px solid transparent;
	border-top: 100px solid red;
}
如果页面中有多个方格那么使用rem可能不会自适应，需要使用百分比单位：vw。长宽都使用vw可以保证正方形，字号也可以使用vw。
大图logo也使用vw可自适应。background-size:100% auto;可以保证图片不变形。
hover：给四个小图标的外层盒子设置，并设置opacity: 0;默认隐藏，之后给四个小图标外层盒子的父元素盒子设置，并设置伪类hover。
小图标的雪碧图：background-size: 有几个图标拼成就写百分之几 auto;background-position: 33.3% 0;如果是横向排列，第一个是0%最后一个100%，中间的安装n-1的数量平分。
flex属性是flex-grow, flex-shrink 和 flex-basis的简写，默认值为0 1 auto。后两个属性可选。flex-grow属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。flex-shrink属性定义了项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。flex-basis属性定义了在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。 http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html。
使用rgba设置颜色子元素不继承父元素设置，可以让子元素独立设置。而opacity会影响子元素的设置。