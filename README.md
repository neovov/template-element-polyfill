# <template> polyfill

A small polyfill to easily use the &lt;template&gt; element.

## Why?

Because.  
Using the &lt;template&gt; element in a browser whom doesn't support it might be a pain, this polyfill fix that (hopefully).  
Using a &lt;template&gt; element within a &lt;template&gt; element might be a hell, but not anymore with this polyfill.  
This polyfill might as well cure cancer but it wasn't tested for.

## How?

Include the template.js file at the end of your document (or do whatever you prefer).
Get the template you want to use, for instance:

```
var template = document.getElementById("my-awesome-template");
```

Use the built-in cloning method (fix a problem with the nested &lt;template&gt; elements):

```
var clone = template.clone();
```

You'll end up with a cloned version of the template (duh!).  
Replace some tokens, some images' URLs or whatever.  
Then, append the content of the template:

```
document.body.appendChild(clone.content);
```

Now, take a sip and win a lot of cash!!1

## Now?

Fork it.