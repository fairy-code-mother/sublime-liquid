# Sublime Snippets for Shopify Development
Sublime preferences and snippets to make Shopify theme development faster.

## Installation
For OSX users, place each snippet you want to use inside `<user>`/Library/Application Support/Sublime Text 3/Packages/User/
Windows or other platforms, you're on your own for the location, but there's enough documentation out there.

## Use
The snippet is called by a series of keys followed by Tab key. In each snippet file, look for `<tabTrigger>` and you will see the keys needed to initiate the snippet. For schema input settings each tag trigger starts with `s` standing for "schema".

## Make it your own
Don't like the tabtrigger keys, or want to modify the snippet? Go for it.

## Contents
- [Basic Schema Input Settings](#basic-schema-input-settings)
- [Specialized Schema Input Settings](#specialized-schema-input-settings)
- [Schema Starter](#schema-starter)
- [Other Liquid Snippets](#other-liquid-snippets)
- [How to edit the Liquid package snippets](#how-to-edit-the-liquid-package-snippets)
- [How to Edit a Color Schemes Syntax Highlighting](#how-to-edit-a-color-schemes-syntax-highlighting)

# Basic Schema Input Settings
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

# Specialized Schema Input Settings
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

# Schema Starter
If you are creating an all new Shopify section this snippet will give you a great starter schema tag with contents.

`sschema` + Tab outputs
```
  {% schema %}
  {
    "name": "",
    "tag": "",
    "class": "",
    "max_blocks": ,
    "settings": [
      
    ],
    "blocks": [
      {
        "name": "",
        "type": "",
        "settings": [
          
        ]
      }
    ],
    "presets": [
      {
        "name": "",
        "blocks": [
          {
            "type": ""
          }
        ]
      }
    ],
    "templates": ["404", "article", "blog", "cart", "collection", "list-collections", "index", "page", "product", "search"]
  }
  {% endschema %}
```

# Other Liquid Snippets
The [Liquid](https://packagecontrol.io/packages/Liquid) package will give you a few starter snippets, but it is not maintained so new tags are not added. Below are new or missing snippets that can be added. Learn how to edit the liquid package [here](#how-to-edit-the-liquid-package-snippets).

**Liquid Literal**

`liq` + Tab outputs
```
  {%- liquid

  

-%}
```

**Render Tag**

`rend` + Tab outputs
```
{%- render '' -%}
```

**Comment Tag**

`comment` + Tab outputs
```
{%- comment -%}

{%- endcomment -%}
```

**Break Tag**

`break` + Tab outputs
```
{%- break -%}
```

**Continue Tag**

`continue` + Tab outputs
```
{%- continue -%}
```

**Raw Tag**

`raw` + Tab outputs
```
{%- raw -%}

{%- endraw -%}
```

# How to Edit the Liquid Package Snippets
The only package that gives you Liquid syntax highlighting is [Liquid](https://packagecontrol.io/packages/Liquid). It also comes with a few snippets. For example using the tab trigger of `assign` in a Liquid HTML file will output `{% assign variable = value %}`, but I wanted to edit some of these snippets to use [whitespace control](https://shopify.dev/api/liquid/basics/whitespace) on the percentage delimeters. I use the `{%-` & `-%}` far more often than without the hyphen so I dont want to keep manually addings those. So here are the steps to edit the default sublime snippets.

1. Default packages resources will not be visible in your Finder. So first you will need to install the [PackageResourceViewer](https://packagecontrol.io/packages/PackageResourceViewer) Sublime package.
2. To open a resource with this package in the Sublime panel type `PackageResourceViewer: Open Resource` > select `Liquid` > select `Snippets/`, here you will see a list of all the default liquid snippets which are…
- assign
- capture
- case
- content_for_layout
- cycle
- for
- if
- ifelse
- include
- named cycle
- unless
- when
3. Select any snippet you want to edit and it will open the file. Make your changes and save.

# How to Edit a Color Schemes Syntax Highlighting
I found most of the Sublime Color Schemes dont highlight liquid syntax in a way thats very readable to me. If you want to edit your chosen color scheme for Liquid and JSON then follow these steps.

1. Go to Sublime Text > Preferences > Customize Color Scheme. 
2. Under rules add a JSON rule for example…
```
 {
   "scope": "",
   "foreground": "HEX COLOR OR CSS COLOR"
 },
```
The scope defines what syntax your changing the color of. For scope here are a few to get you started.
- Liquid Percent Delimeter Begin/End = `punctuation.definition.tag.begin.liquid, punctuation.definition.tag.end.liquid`
- Liquid Curly Bracket Begin/End = `punctuation.definition.object.begin.liquid, punctuation.definition.object.end.liquid`
- Liquid Curly Bracket Inner Contents = `variable.other.liquid`
- Liquid Curly Bracket Inner Underscore = `punctuation.under.separator.liquid`
- Liquid Colons = `punctuation.separator.key-value.liquid`
- Liquid Pipes = `keyword.operator.logical.pipe.liquid`
- Liquid Filters = `support.function.filter.liquid`
- Liquid Strings Begin/End and Contents = `punctuation.definition.string.begin.liquid, punctuation.definition.string.end.liquid, string.quoted.single.liquid, string.quoted.double.liquid`
- Liquid Variables = `variable.other.liquid`
- Liquid Punctuation = `punctuation.separator.liquid`
- JSON Curly Bracket Begin/End = `punctuation.section.mapping.begin.json, punctuation.section.mapping.end.json`
- JSON Brackets Begin/End = `punctuation.section.sequence.begin.json, punctuation.section.sequence.end.json`
- JSON Commas = `punctuation.separator.sequence.json`
- JSON Keys = `meta.mapping.key.json string.quoted.double.json`
- JSON Values = `meta.mapping.value.json string.quoted.double.json`
- JSON Value Commas = `punctuation.separator.mapping.pair.json`
3. Add a rule for each scope you want to recolor and save the file.
