# Custom CSS

```CSS
@import url('https://fonts.googleapis.com/css2?family=Mochiy+Pop+One&display=swap');

.jp {
      font-family: "Mochiy Pop One" !important;
      font-size: 0.9em;
}

@font-face {
    font-family: 'ONE-Mobile-POP';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2105_2@1.0/ONE-Mobile-POP.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: 'ONE-Mobile-POP-B';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2105_2@1.0/ONE-Mobile-POP.woff') format('woff');
    font-weight: 700;
    font-style: normal;
}

@font-face {
    font-family: 'EliceDigitalBaeum_Bold';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_220508@1.0/EliceDigitalBaeum_Bold.woff2') format('woff2');
    font-weight: 400;
    font-style: normal;
}

h1, h2, h3, h4, h5, h6, b {
    font-family: 'ONE-Mobile-POP-B';
}

:root {
    --bg: #efefef;
    --accent: #ff9899;
    --lightpink: #ffd9cd;
}

body#post header, body#subpage header {
    background-color: white;
    margin-bottom: 2em;
}

article {
    background-color: #ffffffd3;
    border-radius: 15px;
    border: 2px dashed var(--accent);
    padding: 2em !important;
}

body {
    font-family: 'ONE-Mobile-POP';
    background-color: var(--bg);
    overflow-x: hidden;
    background-image: linear-gradient(135deg, var(--lightpink) 25%, transparent 25%), linear-gradient(225deg, var(--lightpink) 25%, transparent 25%), linear-gradient(45deg, var(--lightpink) 25%, transparent 25%), linear-gradient(315deg, var(--lightpink) 25%, var(--bg) 25%);
    background-position: 10px 0, 10px 0, 0 0, 0 0;
    background-size: 20px 20px;
    background-repeat: repeat;
}

h1, h2, a, b {
    color: var(--accent) !important;
}

header h1 {
    text-shadow: -2px 0px white, 0px 2px white, 2px 0px white, 0px -2px white;
}

#org-nav, .dropdown-nav, #manage {
    font-family: 'ONE-Mobile-POP' !important;
}

.font.norm, body#collection article.norm, body#post article.norm, body#subpage article.norm, input#title.norm, pre.norm, span.norm, textarea.norm {
    font-family: 'One-Mobile-POP' !important;
}

.book {
    display: none;
}

.action, a.btn, button, input, select.inputform, textarea.inputform {
    font-family: 'One-Mobile-POP' !important;
}

footer hr {
    display: none;
}

table {
    border: 2px solid #ffffff00 !important;
}

th {
    color: var(--accent);
    border-bottom: 2px solid var(--accent) !important;
    border-top: 2px solid #ffffff00 !important;
    border-left: 2px solid #ffffff00 !important;
    border-right: 2px solid #ffffff00 !important;
}

td {
    border-bottom: 2px solid var(--accent) !important;
    border-top: 2px solid #ffffff00 !important;
    border-left: 2px solid #ffffff00 !important;
    border-right: 2px solid #ffffff00 !important;
}

tr {
    border-bottom: 2px solid var(--accent) !important;
}

code, pre {
    border: 0 !important;
    border-radius: 10px !important;
    background-color: var(--lightpink) !important;
    color: #555;
    font-family: 'EliceDigitalBaeum_Bold';
}

@media (max-width: 800px) {
    article {
        width: calc(100% - 50px) !important;
        margin: 10px auto !important;
        padding: 1em !important;
    }
}
```