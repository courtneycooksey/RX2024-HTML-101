# HTML 101

This repository contains the slide deck for the 2024 HTML 101 presentation as well as some code snippets for the examples in the presentation.

Below are the HTML and CSS examples by slide that should be easy to copy into an HTML block or Lava Tester. Examples are separated by slide title.

## Common HTML Tags

### Paragraph

```html
<p>
  Paragraph contents. 
</p>
```

### Header

```html
<h1>
  Big Header 
</h1>
<h6>
  Small Header 
</h6>
```

### Division (Section)

```html
<div>
  Hello World
</div>
```

### Image

```html
<img />
```

### Inline Frame

```html
<iframe></iframe>
```

### Line Break

```html
<br/>
```

### Anchor (Link)

```html
<a>Open Google</a>
```

## Build the Skeleton for a Serving Card

```html
<div>
  <img />
  <div>
    <h3>Serve at Camp!</h3>
    <p>
        Shepherd young hearts and minds to Jesus. Break an 
        arm on the ropes course! You can do it all at camp.
    </p>
    <a>Sign Up</a>
  </div>
</div>
```

## HTML Attributes Provide Information About Elements

### style

```html
<div style="background-color: blue;">Foo</div>
```

### id

```html
<div id="my-special-div">Bar</div>
```

### class

```html
<div class="my-divs">Fizz</div>
```

### src

```html
<img src="https://placebear.com/600/200" />
```

### href (hypertext reference)

```html
<a href="https://google.com">Open Google</a>
```

## Add HTML Attributes to the Card

```html
<div style="border: 1px solid lightgrey;">
  <img src="https://placebear.com/600/300" style="width: 100%;" />
  <div style="padding: 6px;">
    <h3>Serve at Camp!</h3>
    <p>
        Shepherd young hearts and minds to Jesus. Break an 
        arm on the ropes course! You can do it all at camp.
    </p>
    <a class="btn btn-primary" href="https://rock.mychurch.com/Register">Sign Up</a>
  </div>
</div>
```

## The Most Common CSS Selectors

```html
<p id="my-paragraph" class="my-class">Hello!</p>
```

```html
<p class="blue my-class">Hello!</p>
```

```html
<style>
    p {
        color: lightblue;
    }
    #my-paragraph {
        font-weight: bold;
    }
    .blue {
        background-color: blue;
    }
</style>
```

## Combine and Chain Selectors

```html
<p id="my-paragraph" class="my-class">Hello!</p>
```

```html
<p class="blue my-class">Hello!</p>
```

```html
<div class="blue">Hello!</div>
```

```html
<div class="my-class">Hello!</div>
```

```html
<style>
    p {
        color: lightblue;
    }
    #my-paragraph {
        font-weight: bold;
    }
    .blue, p {
        background-color: blue;
    }
    p.blue {
        font-size: 26px; 
    }
</style>
```

## Remove Inline Styling and Add a Card Class

```html
<div class="card">
  <img src="https://placebear.com/600/300" />
  <div>
    <h3>Serve at Camp!</h3>
    <p>
        Shepherd young hearts and minds to Jesus. Break an 
        arm on the ropes course! You can do it all at camp.
    </p>
    <a class="btn btn-primary" href="https://rock.mychurch.com/Register">Sign Up</a>
  </div>
</div>
```

## Define the Style Rules for the Card

```html
<style>
  .card {
    box-shadow: 5px 5px 10px 0px #adadad; 
    /* x-pos, y-pox, blur, spread, color */
    border-radius: 6px; /* round corners */
    overflow: hidden; /* round image corners */
  }
  .card img {
    width: 100%;
  }
  .card div {
    padding: 8px;
  }
</style>
```

## The Grid System Is Defined by Rows and Columns

```html
<div class='row'>
    <div class='col-xs-2'>Col-2</div>
    <div class='col-xs-6'>Col-6</div>
    <div class='col-xs-4'>Col-4</div>
</div>
```

## Create a Responsive Row of Cards

```html
<div class="row">
  <div class="col-xs-12 col-md-4">
    <div class="card">
      <img src="https://placebear.com/600/300" />
      <div>
        <h3>Serve at Camp!</h3>
        <p>...</p>
        <a class="btn btn-primary" href="https://rock.mychurch.com/Register">Sign Up</a>
      </div>
    </div>
  <div class="col-xs-12 col-md-4"> ...Card Two... </div>
  <div class="col-xs-12 col-md-4"> ...Card Three... </div>
</div>
```

## You Can Use CSS in an Email

```html
<div style="display: flex;">
  <div style="width: 50%;">Hello</div>
  <div style="width: 50%;">World</div>
</div>
```
