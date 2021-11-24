# Sublime Snippets for Shopify Dev
Sublime preferences and snippets to make Shopify theme development faster.

## Installation
For OSX users, place each snippet you want to use inside `<user>`/Library/Application Support/Sublime Text 3/Packages/User/
Windows or other platforms, you're on your own for the location, but there's enough documentation out there.

## Use
The snippet is called by a series of keys followed by Tab key. In each snippet file, look for `<tabTrigger>` and you will see the keys needed to initiate the snippet. For schema input settings each tag trigger starts with `s` standing for "schema".

## Make it your own
Don't like the tabtrigger keys, or want to modify the snippet? Go for it.

## Contents

### Basic Schema Input Settings
**Checkbox**

`scheckbox` + Tab outputs
```
 {
    "type": "checkbox",
    "id": "",
    "label": "",
    "default": 
  }
```
**Number**

`snumber` + Tab outputs
```
 {
    "type": "number",
    "id": "",
    "label": "",
    "default": 
  }
```
**Radio**

`sradio` + Tab outputs
```
 {
    "type": "radio",
    "id": "",
    "label": "",
    "options": [
      {
        "value": "",
        "label": ""
      }
    ],
    "default": ""
  }
```
**Range**

`srange` + Tab outputs
```
 {
    "type": "range",
    "id": "",
    "min": ,
    "max": ,
    "step": ,
    "unit": "",
    "label": "",
    "default": 
  }
```
**Select**

`sselect` + Tab outputs
```
  {
    "type": "select",
    "id": "",
    "label": "",
    "options": [
      {
        "value": "",
        "label": ""
      },
      {
        "value": "",
        "label": ""
      },
      {
        "value": "",
        "label": ""
      }
    ],
    "default": ""
  }
```
**Text**

`stext` + Tab outputs
```
  {
    "type": "text",
    "id": "",
    "label": "",
    "default": ""
  }
```
**Textarea**

`stext` + Tab outputs
```
  {
    "type": "textarea",
    "id": "",
    "label": "",
    "default": ""
  }
```

### Specialized Schema Input Settings
**Article**

`sarticle` + Tab outputs
```
 {
    "type": "article",
    "id": "",
    "label": "Article"
  }
```
**Blog**

`sblog` + Tab outputs
```
 {
    "type": "blog",
    "id": "",
    "label": "Blog"
  }
```
**Collection**

`scollection` + Tab outputs
```
   {
    "type": "collection",
    "id": "",
    "label": "Collection"
  }
```
**Page**

`spage` + Tab outputs
```
  {
    "type": "page",
    "id": "",
    "label": ""
  }
```
**Product**

`sproduct` + Tab outputs
```
  {
    "type": "product",
    "id": "",
    "label": ""
  }
```
**Color**

`scolor` + Tab outputs
```
  {
    "type": "color",
    "id": "",
    "label": "",
    "default": "#"
  }
```
**Font Picker**

`sfont` + Tab outputs
```
  {
    "type": "font_picker",
    "id": "",
    "label": "",
    "default": "#"
  }
```
**HTML**

`shtml` + Tab outputs
```
  {
    "type": "html",
    "id": "",
    "label": ""
  }
```
**Image Picker**

`simage` + Tab outputs
```
  {
    "type": "image_picker",
    "id": "",
    "label": ""
  }
```
**Linklist**

`slinklist` + Tab outputs
```
  {
    "type": "link_list",
    "id": "",
    "label": ""
  }
```
**Liquid**

`sliquid` + Tab outputs
```
  {
    "type": "liquid",
    "id": "",
    "label": "",
    "default": ""
  }
```
**Richtext**

`srichtext` + Tab outputs
```
  {
    "type": "richtext",
    "id": "",
    "label": ""
  }
```
**Url**

`surl` + Tab outputs
```
  {
    "type": "url",
    "id": "",
    "label": ""
  }
```
**Video URL**

`svideo` + Tab outputs
```
  {
    "type": "video_url",
    "id": "",
    "label": "",
    "accept": [
      "youtube",
      "vimeo"
    ]
  }
```
