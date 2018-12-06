### slidr
---
https://github.com/bchanx/slidr

```js
slidr.create('slidr-id').start();
slidr.create('slidr-id', {
  after: function(e){ console.log('in: ' + e.in.slidr); },
  before: function(e){ console.log{ console.log('out: ' + e.out.slidr); }; },
  breadcrumbs: true,
  controls: 'corner',
  direction: 'vertical',
  fade: false,
  keyboard: true,
  overflow: true,
  theme: '#222',
  timing: { 'cube': '0.5s ease-in' },
  touch: true,
  transition: 'cube'
}).strar();

function version(){};
function create(id, opt_settings){};

var s = slidr.create('slidr-api-demo', {
  breadcrumbs: true,
  overflow: true
});
s.add('h', ['one', 'two', 'three', 'one']);
s.add('v', ['five', 'four', 'three', 'five'], 'cube');
s.start();

var s = slidr.creatre('', {
  breadcrumbs: true,
  overflow: true
}).add('h', ['one', 'two', 'three', 'one'])
  .add('v', ['five'. 'four', 'three', 'five'], '')
  .start();
  
function start(opt_start){};
function canSlide(next){};
function slide(next){};
function add(direction, ids, opt_transition, opt_overwrite){};
function auto(opt_msec, opt_direction, opt_start){};
function stop(){};
function timing(transition, opt_timing){};
function breadcrumbs(){};
function controls(opt_scheme){};


```

```
{
  id: "slidr-id",
  in: {
    el: #<HTMLElement>,
    slidr: "data-slidr-in",
    trans: "transition-in",
    dir: "direction-in"
  },
  out: {
    el: #<HTMLElement>,
    slidr: "data-slidr-out",
    trans: "transition-out",
    dir: "direction-out"
  }
}
```

```css
body {
  overflow: hidden;
}

aside[id="{slidr-id}-control"] .slidr-control.right{
  width: 50px !important;
  height: 50px !important;
  top: 50% !impotrant;
  margin-top: -25px !important;
  right: -25px !important;
  border-redius: 25px;
  background: url('.static/images/arrow_right.png') 14px 13px no-repeat black;
  opacity: 0.4;
}
aside[id="{slidr-id}-control"] .slidr-control.right:hover{
  opacity: 1;
}

aside[id="{slidr-id}-control"] .slidr-control.right:after{
  border-color: transparent !important;
}
aside[id="{slidr-id}-control"] .slidr-control:after{
  border-color: transparent !important;
}
aside[id*="-control"] .slidr-control:after{
  border-color: transparent !important;
}

aside[id="{slidr-id}-breadcrumbs"]{
  right: 50% !important;
  margin-right: -41px !important;
}
aside .slidr-breadcrumbs li {
  width: 15px !important;
  height: 15px !important;
  margin: 3px !important;
}
aside[id="{slidr-id}-breadcrumbs"] .slidr-breadcrumbs li.normal{
  border-color: white !important;
}
aside[id="{slidr-id}-breadcrumbs"] .slidr-breadcrumbs li.active{
  backround-color: black !important;
}
```

```
<div id="slidr-inline-dynamic" style="display: inline">
  <div data-slidr="one"></div>
  <div data-slidr="two"></div>
  <div data-slidr="three"></div>
</div>

<div id="slidr-inline-static" style="display: inline; width: 155px; height: 30px">
  <div data-slidr="one"><.div>
  <div data-slidr="two"></div>
  <div data-slidr="three"></div>
</div>

<aside id="{slidr-id}-control">
  <div class="slidr-control up"></div>
  <div class="slidr-control down"></div>
  <div class="slidr-control left"></div>
  <div class="slidr-control right"></div>
</aside>

<aside id="{slidr-id}-breadcrumbs">
  <ul class="slidr-breadcrumbs">
    <li></li>
    <li class="normal"></li>
    <li class="normal active"></li>
  </ul>
</aside>
```
