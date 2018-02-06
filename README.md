# Jparallax
Powered by 
Rodrigo Jarouche

The easiest way to animate your parallax layoult

  - Simple Sintax
  - Little or no configuration
  - See the Magic

## Motivation
Make easy put animations in parallax layoults

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
<div class="jar_bounce">test</div>
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
<div class="divAnime" >test</div>
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
            /* Prefix of the classe for animation ex. if you put foo_ the class to animate bounceIn is foo_, jar_ is default */
            prefix  : 'jar_',
            /* Put the animation direction when up the page , true is default*/
            default_inverted_animation  : true,
            /* Offset of the page, defined by jquery waypoints https://github.com/imakewebthings/waypoints , 85% is default*/
            offset  : "85%"
      });
    });
</script>  

<body>
<div class="jar_bounce" ></div>
</body>
```

In this case All animations is listed on [animate-css](http://daneden.me/animate), to use this method just put prefix + animation in the class. 
Example, you want to use the fadeIn animation in a span, put the class jar_fadeIn.
**DO NOT FORGET** TO PUT THE jParallax.start in the javascript!

But, if you prefer to use the **addAnimation** jQuery extension, this configuration has no effect, the configuration must be passed by parameter
```html
        $('.divAnime').addAnimation('fadeInUp',true,'85%');
```
Being the parameters
  - Animation name, exactly the name listed on [animate-css](http://daneden.me/animate) 
  - Inverted Animation.Values true ou false Put the animation direction when up the page , true is default. 
  - Offset of the page, defined by jquery waypoints https://github.com/imakewebthings/waypoints , 85% is default

## License
MIT LICENSE
