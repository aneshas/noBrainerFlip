noBrainerFlip
=============

Simple lightweight jQuery flip plugin

Usage

- First of all, you need to have an element which you want to apply flip to, let us assume it is a div element with a class name of your choosing, "flip-container" for example which should have width and height css properties set up.

1:  <div class="flip-container">  
2:    <img src="http://lorempixel.com/150/150">  
3:  </div>  

Css

  
1:  .flip-container {  
2:    width: 150px;  
3:    height: 150px;  
4:  }  

- Other thing that is important is that all content inside this flip element should have their width and height set to 100% for best effect. In this example we have only img element inside flip-container, so we set its width and height to 100%

1:  .flip-container img {  
2:    width: 100%;  
3:    height: 100%;  
4:  }  

- Finally you need to initialize noBrainerFlip and you are ready to go.

Simple initialization
1:  <script>  
2:      $(document).ready(function() {  
3:        $("div.flip-container").noBrainerFlip();  
4:      });  
5:  </script>  

Initialization with some custom options
1:  <script>  
2:      $(document).ready(function() {  
3:        $("div.flip-container").noBrainerFlip({  
4:          flipContent: '<img src="http://lorempixel.com/150/150?xyz" />', //Optional - Use if you want to fill container with different content after flip  
5:          inSpeed: 200, //Optional - Flip in speed in ms, default: 200  
6:          outSpeed: 200, //Optional - Flip out speed in ms - default: 200  
7:          setCursor: true //Optional - Sets cursor to pointer - default: false  
8:        });  
9:      });  
10:  </script>  
