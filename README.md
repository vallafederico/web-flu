# Web-flu
Things for Webflow but in a form that works for everything! Missing pieces, snippets, fully fledged extensions, plugins kinda things. In no particular order, mostly sparked from project needs. Couldn't really think of a better name and now we're stuck here :).

> I like no code but with some code in it. *- Someone*

[Cloneables in action here!](https://webflow.com/vallafederico)

## Community & Bugs
[Issues](https://github.com/vallafederico/web-flu/issues) are there to report bugs, and hopefully stuffs can get fixed.    
[Discussion](https://github.com/vallafederico/web-flu/discussions) is there to share, suggest and all the rest.

## Contribute
Have developed a codebase for useful webflow things? Care to share? We'd love to have you here. 
Do it [here!](https://github.com/vallafederico/web-flu/discussions/2).



Have code skills? Help a no-code bro realise his dreams and fix some [issues](https://github.com/vallafederico/web-flu/issues) while he keeps saying he doesn't need any code to make his websites!



## Content of this repo
**Main** has the uncompiled, class based original code. From here you can pull stuffs to integrate on your own codebase if that's the way you use Webflow!

**Dist** has the compiled, minified (when I do not forget), single instance code. It's the right one to to re-save as a .txt to store in webflow's project assets, or to use if only a single one is needed.

**Modules** Contains the code in library form, available for Browser imports.


## How to

### ESM Modules
*In library form with available imports.*   
Before */body*, simply add a `script type="module"`, import the thing/s you want to call. Initialise it with the `new` keyword. Refer to the related docs to find the proper configuration or check the defaults.

```html

<script type="module">
  import { Something } from 'LIBRARY-LINK'
  
  new Something({
    //... config here
  })
</script>

```

### Via Webflow's assets
*Using a .js.txt file hosted in the webflow project.*   
This is the safer & preferred version for shipped, finalised projects. I'm not sure everything will be maintained, and can't assure backwards compatibility (I'll try though). You should download the js file, re-save it as a **.js.txt** (this way you can upload it to webflow as an asset). Once uploaded to the webflow assets, get the link and use it as the above.

```html

<script type="module">
  import { Something } from 'WF-ASSET-LINK'
  
  new Something({
    //... config here
  })
</script>

```

### Via CodeSandbox
*Pulling the live code through codesandbox.*     
This one is not available on every snippets, as some I'm bundling locally before shipping. Still, most of those will be available on Codesandbox for you to fiddle with the code as well. In this case the code will be brought in via a basic `<script src="LINK"></script>`. Fork it and try to change something.


### The code way!
*This is my preferred method, though might be not viable for your workflow.*      
The uncompiled code can be found on the main branch, neatly packages as a js Class for you to be inegrated in your code base.
