# Web-flu
Things for Webflow but in a form that works for everything! Missing pieces, snippets, fully fledged extensions, plugins kinda things. In no particular order, mostly sparked from project needs.

[Webflow Public](https://webflow.com/vallafederico)


## How to

### ESM Modules
*In library form with available imports.*   
Before */body*, simply add a `script type="module"`, import the thing/s you want to call. Config it on call (if the defaults are not right). Refer to the related docs to find the proper configuration.

```html

<script type="module">
  import { Something } from 'LIBRARY-LINK'
  
  new Something({
    //... config here
  })
</script>

```

### Through Webflow
*Using a .js.txt file hosted in the webflow project.*   
This is the safer preferred version 
