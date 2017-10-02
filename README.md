# Jparallax
Powered by 
[![](https://2.bp.blogspot.com/-4OrZe3SvEio/Wa3wtXDOU_I/AAAAAAAACuk/h0jvaRoJUYgsSJTiIT7d9wmHD50GF9DOACEwYBhgL/s1600/logo_vertical.png)](http://rodrigojarouche.blogspot.com.br/)

The easiest way to animate your parallax layoult

  - Simple Sintax
  - Little or no configuration
  - See the Magic
 
## Code Example

Class Method
```html
<script src="js/jquery.js"></script>  
<script src="js/jquery.waypoints.js"></script>
<script src="js/jarouche_parallax.js"></script>
<link rel="stylesheet" href="css/animate.css-master/animate.css"> 

<script>
        $(function(){
                jParallax.start();
    });
</script>  

<body>
<div class="jar_bounce" ></div>
</body>
```

or use the **addAnimation** jQuery extension

```html
<script src="js/jquery.js"></script>  
<script src="js/jquery.waypoints.js"></script>
<script src="js/jarouche_parallax.js"></script>
<link rel="stylesheet" href="css/animate.css-master/animate.css"> 

<script>
        $(function(){
                $('.divAnime').addAnimation('fadeInUp');
    });
</script>  

<body>
<div class="divAnime" ></div>
</body>
```


## Dependences

  - Minimum jQuery v2.2.4 (included in this package)
  - [jQuery Waypoints](https://github.com/imakewebthings/waypoints/) (included in this package) 
  - Jparallax use a modifield version of [animate-css](http://daneden.me/animate) (included in this package)

## Configuration
If you are you using the class method you can configure the  jParallax.start(); like this
```html
<script src="js/jquery.js"></script>  
<script src="js/jquery.waypoints.js"></script>
<script src="js/jarouche_parallax.js"></script>
<link rel="stylesheet" href="css/animate.css-master/animate.css"> 

<script>
        $(function(){

    jParallax.start({
            /* Prefix of the classe for animation ex. if you put foo_ the class to animate bounceIn is foo_ */
            prefix  : 'jar_',
            /* Put the animation direction when up the page */
            default_inverted_animation  : true,
            /* Offset of the page, defined by jquery waypoints https://github.com/imakewebthings/waypoints */
            offset  : "85%"
      });
    });
</script>  

<body>
<div class="jar_bounce" ></div>
</body>
```

In this case All animations is listed on [animate-css](http://daneden.me/animate), to use this method just put

  
