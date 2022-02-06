# What is in the head
The **head** of the HTML is not displayed in the browser, but contains information about the metadata, linking CSS and others that will describe your site.

```html
<head>
  <meta charset="utf-8">
  <title>The title of the page </title>
</head>
```

### Title element
(*self-explanatory*)

# Meta element
**Metadata** - data that describes a data. 

### character encoding
- Sets the HTML character encoding.

```html
<!-- UTF-8 is a standard where latin and other scripts can be read. -->
<meta charset="utf-8">
<!-- Setting the charset standard to `ISO-8859-1` will only read the latin characters, other characters like japanese characters will be read as garbage by the browser. -->
```

### author and description
The `<meta>` element may contain attributes like:
- `name` - specifies what type of meta.
- `content` - the actual meta content

```html
<meta name="author" content="Natsurii">
<meta name="description" content="This metadata describes what the site what are you making at.">
```
Specifying author will able to understand who wrote the page, while specifying description will help to improve site's SEO. 

# Other types of metadata

### Open Graph Data
is a metadata protocol from Facebook which invented for richer metadata for sites.

```html
<meta property="og:image" content="https://developer.mozilla.org/static/img/opengraph-logo.png">
<meta property="og:description" content="The Mozilla Developer Network (MDN) provides
information about Open Web technologies including HTML, CSS, and APIs for both Web sites
and HTML5 Apps. It also documents Mozilla products, like Firefox OS.">
<meta property="og:title" content="Mozilla Developer Network">
```

### Favicon
moniker for *"Favorites icon"*. Which use to show the icon of the site when bookmarked.

```html
<!-- The favicon should be in .ico format for better compatibility. -->
<link rel="icon" href="favicon.ico" type="image/x-icon">
```
Other types of favicon should be consider as well.
```html
<!-- third-generation iPad with high-resolution Retina display: -->
<link rel="apple-touch-icon-precomposed" sizes="144x144" href="https://developer.mozilla.org/static/img/favicon144.png">
<!-- iPhone with high-resolution Retina display: -->
<link rel="apple-touch-icon-precomposed" sizes="114x114" href="https://developer.mozilla.org/static/img/favicon114.png">
<!-- first- and second-generation iPad: -->
<link rel="apple-touch-icon-precomposed" sizes="72x72" href="https://developer.mozilla.org/static/img/favicon72.png">
<!-- non-Retina iPhone, iPod Touch, and Android 2.1+ devices: -->
<link rel="apple-touch-icon-precomposed" href="https://developer.mozilla.org/static/img/favicon57.png">
<!-- basic favicon -->
<link rel="icon" href="https://developer.mozilla.org/static/img/favicon32.png">
```

### Applying CSS and Javascript
Applying CSS and Javascript is possible using the `<link>` and `<script>` element.

```html
<link rel="stylesheet" href="my-css-file.css">
<script src="my-js-file.js" defer></script>
```

### Document primary language
This ensure that the page indexed effectively by SEO.
```html
<html lang="en-US"></html>
```
Can be also set a different language in the subsection of document.

```html
<p>Japanese example: <span lang="ja">ご飯が熱い。</span>.</p>
```








