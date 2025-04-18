![GitHub stars](https://img.shields.io/github/stars/Parsegan/MetaKit?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/Parsegan/MetaKit?style=flat-square)
![License](https://img.shields.io/github/license/Parsegan/MetaKit?style=flat-square)


# MetaKit. an HTML snippet. 💚💙

> The ultimate HTML `<head>` starter. Built for SEO, accessibility, and real-world dev flow.

## ✅ Features

- Perfect `<html>` + `<head>` setup for modern websites

- SEO-optimized, accessibility-aware, and fully commented

- Includes Open Graph, Twitter Cards, schema.org JSON-LD, and more

- Ideal for portfolios, blogs, PWAs, and client projects

## 🚀 How to Use

1. Copy the full contents of [THIS HTML File]([./index.html]) ✔**with comments**

2. Paste it into your HTML file

3. Customize content-specific fields (`title`, meta, social links, etc.)

4. You can also copy content of [THIS HTML File]([./index.min.html]) ❌**without comments**

## 🧩 Includes

- `<meta>` best practices

- Responsive design setup

- Social media previews

- Multilingual SEO support

- PWA + Apple mobile settings

## 🚀 How to Use MetaKit Snippet in Your Code Editor

Turn MetaKit into a reusable, auto-completing snippet in under 1 minute!

### 🔧 1. Use This Snippet Generator Tool

👉 Open the online snippet generator:  

[**snippet-generator.app**](https://snippet-generator.app/?description=&tabtrigger=&snippet=&mode=vscode)

Then:

1. Paste MetaKit code into the large `snippet` box.

2. Give your snippet a description (e.g., `SEO-friendly HTML Head Setup`).

3. Set a trigger keyword (like `metakit`, `headmeta`, etc.).

4. Select your editor from the mode dropdown — supports:

   - `Visual Studio Code`

   - `Sublime Text`

   - `Atom`

5. Copy the final snippet from the output box at the bottom.

6. now paste the trigger keyword you did setup in any HTML file and you shall see the snippet 😘

---

### 🧪 2. Add the Snippet to Your Editor

#### ✅ For VS Code:

1. Open your editor and go to:  

   `File → Preferences → Configure User Snippets`

2. Select:

   - `New Global Snippets file` or

   - A language-specific one (like `html.json`)

3. Name it (e.g., `metakit-snippets.code-snippets`)

4. Paste the snippet you copied

5. Save — you're done!

> 🔁 Now type your trigger keyword (e.g. `metakit`) inside an HTML file — the full MetaKit snippet will autocomplete!

---

<div class="" role="region" tabindex="0">
<table>
    <caption>
        <h3>🧠 What Each Field Means</h3>
    </caption>
    <thead>
        <tr>
            <th>Field</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>description</td>
            <td>Optional name shown in the suggestion dropdown</td>
        </tr>
        <tr>
            <td>prefix</td>
            <td>The trigger word you type to activate the snippet</td>
        </tr>
        <tr>
            <td>body</td>
            <td>The actual code snippet, line-by-line</td>
        </tr>
    </tbody>
</table>
</div>





### ✨ Tips

- Use a short and easy prefix like `mhead`, `kithead`, or `metakit`

- Snippets can be reused across multiple projects.

- Create variations (e.g., only OG tags or minimal SEO) using different prefixes.



# 📚 MetaKit: Annotated HTML Head Boilerplate

This guide explains what each part of `Index.html` does, referencing approximate line numbers and the why behind them.


## 🧠 Basic HTML Structure


```html
  <!DOCTYPE html>
  <html lang="en" dir="ltr" translate="no">
```

-   Declares the document as HTML5.

-   `lang="en"` helps screen readers & SEO.

-   `dir="ltr"` sets text direction (use `rtl` for Arabic/Hebrew).

-   `translate="no"` prevents Google Translate from changing fixed UI text (e.g., navs or buttons).



## 🌐 Alternate Languages


```html
<link rel="alternate" href="https://example.com/" hreflang="en" />
<link rel="alternate" href="https://example.com/fr" hreflang="fr" />
<link rel="alternate" href="https://example.com/de" hreflang="de" />
<link rel="alternate" href="https://example.com/" hreflang="x-default" />
```

-   Supports multilingual sites by guiding search engines to the correct version of your content.



## 📦 Encoding and Compatibility

```html
<meta charset="UTF-8" />
<meta http-equiv="Content-Language" content="en" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
```

-   UTF-8 handles all languages/symbols.

-   `viewport` makes it responsive.

-   `X-UA-Compatible` ensures compatibility with legacy IE.



## 🔐 Security & Privacy

```html
<meta http-equiv="Content-Security-Policy" content="..." />
```

 *   Controls what resources can load (scripts, styles, fonts).
     
 *   Defends against XSS attacks.
     
 *   Be careful not to block important assets.
     



## 🍎 Apple-Specific Meta

```html
<meta name="apple-mobile-web-app-capable" content="yes" />
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
```

 *   Makes the web app look full-screen on iOS.
     
 *   Sets status bar to blend with background.
     



## 📈 SEO & Indexing

```html
<meta name="description" content="..." />
<meta name="robots" content="index, follow" />
<meta name="keywords" content="..." />
```

 *   `description` appears in Google search.
     
 *   `robots` tells crawlers to index and follow links.
     
 *   `keywords` still used by some minor engines (optional).
     



## 🎯 Social Sharing Metadata

### Open Graph (Facebook, LinkedIn, etc.)

```html
<meta property="og:title" content="..." />
<meta property="og:description" content="..." />
<meta property="og:image" content="..." />
```

 *   Controls how the site appears in social media previews.
     
 *   `og:image` should be 1200x630 px.
     

### Twitter Cards

```html
<meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:app:name:googleplay" content="" />
    <meta name="twitter:app:url:googleplay" content="" />
    <meta name="twitter:app:id:googleplay" content="" />
    <meta name="twitter:app:name:iphone" content="" />
    <meta name="twitter:app:url:iphone" content="" />
    <meta name="twitter:app:id:iphone" content="" />
    <meta name="twitter:app:name:ipad" content="" />
    <meta name="twitter:app:url:ipad" content="" />
    <meta name="twitter:app:id:ipad" content="" />
    <meta name="twitter:site" content="@YourTwitterHandle" />
    <meta name="twitter:creator" content="@YourTwitterHandle" />
    <meta
      name="twitter:title"
      content="A.N. Author | Captivating Books & Illustrations"
    />
    <meta
      name="twitter:description"
      content="Discover captivating books and illustrations by A.N. Author. Explore genres, stories, and artwork in one immersive experience."
    />
    <meta name="twitter:image" content="https://www.example.com/sample.jpg" />
    <meta
      name="twitter:image:alt"
      content="A preview of captivating books and illustrations by A.N. Author."
    />
```

 *   Enables large preview when sharing on Twitter.
     
 *   Add handle with `@YourTwitterHandle`.
     



## 👤 Author & JSON-LD Structured Data

```html
<meta name="author" content="..." />
<script type="application/ld+json">...</script>
```

 *   Declares the author.
     
 *   JSON-LD is used by Google for rich results in search.
     



## 🎨 Theming & Color Scheme

```html
<meta name="color-scheme" content="light dark" />
<meta name="theme-color" content="#ffffff" />
```

 *   Enables proper dark/light mode rendering.
     
 *   Sets browser UI theme on mobile.
     

## 🧠 Performance & UX Enhancers

### Fonts and Styles

```html
<link rel="preload" href="..." as="..." />
<link rel="stylesheet" href="..." />
```

 *   Preloads important assets (fonts, styles, images).
     
 *   `rel="preload"` gives browser a heads-up.
     

### Icons and PWA

```html
<link rel="apple-touch-icon" href="..." />
<link rel="manifest" href="/site.webmanifest" />
```

 *   Adds favicons and PWA manifest for installable apps.
     



## 🔠 Canonical & SEO Boost

```html
<link rel="canonical" href="https://www.example.com" />
```

 *   Prevents SEO penalties for duplicate content.
     

## ⚙️ Scripts

```html
<script type="module" src="..." />
<script async src="..." />
```

 *   `type="module"` is modern JS.
     
 *   `async` speeds up load without blocking DOM.
     
## 🚫 Fallback

```html
<noscript>...</noscript>
```
*   Displays a message if JavaScript is disabled.


## 🤝 Contributors

Big thanks to everyone helping improve MetaKit!

Whether you’re fixing typos, suggesting new tags, improving performance, or translating—every bit helps.

### Want to contribute?

1. Fork the repo 🍴  

2. Make your edits ✍️  

3. Submit a pull request 🔁  

Check out [`CONTRIBUTING.md`](./CONTRIBUTING.md) for full guidelines.

💡 All contributions are welcome—code, feedback, ideas, docs, or design.

Made with ❤️ by [@Parsegan](https://github.com/Parsegan)


## 🔍 Preview

![](/Preview)

## 🛡 License

MIT

