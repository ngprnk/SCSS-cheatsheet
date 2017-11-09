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
  @mixin border-radius($radius){
    -moz-border-radius: $radius;
    -webkit-border-radius: $radius;
  }

  button {
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

## Nesting
```scss 

// Elements can be Nested like so
.container{
  a{
    color: red;
  }
}

```

## Parent Selectors

```scss
  a{
    color: white;
    &:hover: {text-decoration: underline;}
  }


```