# SCSS CheatSheet

## Variables

```scss
$primary-color: #3498db;
$secondary-color: #2ecc71;
```

## Partials

```scss

// reset.css
  body, html, h1, h2, h3, h4, h5, h6{
    margin: 0;
    padding: 0;
  }

// main.css

@import 'reset'; // import partials using @import 'filenamne'
body{
  font: Helvetica Neue;
}

```

## Mixins 

```scss 
  @mixin border-radius ($color){
     -webkit-border-radius: $radius;
     -moz-border-radius: $radius;
      -ms-border-radius: $radius;
          border-radius: $radius;
  }

  .box {
      @include border-radius(10px);
    }

```

## Extend/ Inheritance

```scss
 .button{
   height: 10px;
   width: 60px;
   border: 1px solid red;
 }

 .button-success{
   @extend .button;
   background-color: green;
 }


```