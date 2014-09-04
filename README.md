noBrainerFlip
=============

Simple lightweight jQuery flip plugin

<h3>
Usage</h3>
<div>
<br /></div>
<div>
- First of all, you need to have an element which you want to apply flip to, let us assume it is a div element with a class name of your choosing, "flip-container" for example which should have width and height css properties set up.<br />
<br />
<pre style="background-image: URL(http://2.bp.blogspot.com/_z5ltvMQPaa8/SjJXr_U2YBI/AAAAAAAAAAM/46OqEP32CJ8/s320/codebg.gif); background: #f0f0f0; border: 1px dashed #CCCCCC; color: black; font-family: arial; font-size: 12px; height: auto; line-height: 20px; overflow: auto; padding: 0px; text-align: left; width: 99%;"><code style="color: black; word-wrap: normal;">1:  &lt;div class="flip-container"&gt;  
2:    &lt;img src="http://lorempixel.com/150/150"&gt;  
3:  &lt;/div&gt;  
</code></pre>
<br />
Css<br />
<br />
<pre style="background-image: URL(http://2.bp.blogspot.com/_z5ltvMQPaa8/SjJXr_U2YBI/AAAAAAAAAAM/46OqEP32CJ8/s320/codebg.gif); background: #f0f0f0; border: 1px dashed #CCCCCC; color: black; font-family: arial; font-size: 12px; height: auto; line-height: 20px; overflow: auto; padding: 0px; text-align: left; width: 99%;"><code style="color: black; word-wrap: normal;">  
1:  .flip-container {  
2:    width: 150px;  
3:    height: 150px;  
4:  }  
</code></pre>
<br /></div>
<div>
- Other thing that is important is that all content inside this flip element should have their width and height set to 100% for best effect. In this example we have only img element inside flip-container, so we set its width and height to 100%<br />
<br />
<pre style="background-image: URL(http://2.bp.blogspot.com/_z5ltvMQPaa8/SjJXr_U2YBI/AAAAAAAAAAM/46OqEP32CJ8/s320/codebg.gif); background: #f0f0f0; border: 1px dashed #CCCCCC; color: black; font-family: arial; font-size: 12px; height: auto; line-height: 20px; overflow: auto; padding: 0px; text-align: left; width: 99%;"><code style="color: black; word-wrap: normal;">1:  .flip-container img {  
2:    width: 100%;  
3:    height: 100%;  
4:  }  
</code></pre>
<br /></div>
<div>
- Finally you need to initialize noBrainerFlip and you are ready to go.<br />
<br />
<h4>
Simple initialization</h4>
</div>
<div>
<pre style="background-image: URL(http://2.bp.blogspot.com/_z5ltvMQPaa8/SjJXr_U2YBI/AAAAAAAAAAM/46OqEP32CJ8/s320/codebg.gif); background: #f0f0f0; border: 1px dashed #CCCCCC; color: black; font-family: arial; font-size: 12px; height: auto; line-height: 20px; overflow: auto; padding: 0px; text-align: left; width: 99%;"><code style="color: black; word-wrap: normal;">1:  &lt;script&gt;  
2:      $(document).ready(function() {  
3:        $("div.flip-container").noBrainerFlip();  
4:      });  
5:  &lt;/script&gt;  
</code></pre>
</div>
<div>
<br /></div>
<h4>
Initialization with some custom options</h4>
<pre style="background-image: URL(http://2.bp.blogspot.com/_z5ltvMQPaa8/SjJXr_U2YBI/AAAAAAAAAAM/46OqEP32CJ8/s320/codebg.gif); background: #f0f0f0; border: 1px dashed #CCCCCC; color: black; font-family: arial; font-size: 12px; height: auto; line-height: 20px; overflow: auto; padding: 0px; text-align: left; width: 99%;"><code style="color: black; word-wrap: normal;">1:  &lt;script&gt;  
2:      $(document).ready(function() {  
3:        $("div.flip-container").noBrainerFlip({  
4:          flipContent: '&lt;img src="http://lorempixel.com/150/150?xyz" /&gt;', //Optional - Use if you want to fill container with different content after flip  
5:          inSpeed: 200, //Optional - Flip in speed in ms, default: 200  
6:          outSpeed: 200, //Optional - Flip out speed in ms - default: 200  
7:          setCursor: true //Optional - Sets cursor to pointer - default: false  
8:        });  
9:      });  
10:  &lt;/script&gt;  
</code></pre>
<div>
<br /></div>
<div>
<br /></div>
<div>

<a href="http://jsfiddle.net/AnesHasicic/zgcgLt45/">JsFiddle Example</a>
