![spp.js logo](https://raw.github.com/flashhawk/spp.js/dev/logo.png)
======
### Welcome Spp.js
Spp.js is a sample physics particle system engine for javascript.

### Feature

* Code less, simple structure.
* Based on classical Newtonian mechanics.
* Make your own custom forces or particles
* Easy to build interactive projects.
* Open source!

### Getting Started
```html
<script src="js/spp.min.js"></script>
```

```html
<script>
        var ps=new SPP.ParticleSystem();
        var particle=ps.createParticle(SPP.Particle);
        particle.life=3;
        particle.position.x=50;
        particle.position.y=60;
        particle.addForce("someForceName",someForce);
        particle.onUpdate=someUpdateHander;
        //particle.addEventListener("dead",deadHandler);
        particle.on("dead",deadHandler);
        animate();
        ps.start();
        
        function someUpdateHander()
        {
                ...
        };
        function deadHandler(event)
        {
                ...
        };
        
        function animate()
        {
               requestAnimationFrame(animate);
               ps.render();
               ...
        } 
<script>
```
### Examples
* [gettingStarted](http://flashhawk.github.com/spp.js/examples/gettingStarted/)
* [spriteImage](http://flashhawk.github.com/spp.js/examples/spriteImage/)
* [easelJS](http://flashhawk.github.com/spp.js/examples/easelJS/)
* [attraction](http://flashhawk.github.com/spp.js/examples/attraction/)
* [repulsion](http://flashhawk.github.com/spp.js/examples/repulsion/)

### Game
* [fruitNinja](http://flashhawk.github.com/spp.js/examples/fruitNinja/)
* [斩立觉](https://itunes.apple.com/cn/app/zhan-li-jue/id636378939?ls=1&mt=8)


### Support or Contact
Weibo: http://weibo.com/flashawk? or contact flashhawkmx@gmail.com and we’ll help you sort it out.
