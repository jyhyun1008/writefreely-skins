# Custom CSS

```CSS
@font-face {
    font-family: 'Cafe24Shiningstar';
    src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/noonfonts_twelve@1.1/Cafe24Shiningstar.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: 'NanumSquareRound';
    src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/noonfonts_two@1.0/NanumSquareRound.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: 'intelone-mono-font-family-italic';
    src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/noonfonts_2307-1@1.1/intelone-mono-font-family-italic.woff2') format('woff2');
    font-weight: 400;
    font-style: normal;
}

:root {
    --fg: rgb(89, 77, 71);
    --fglight: rgb(133, 115, 105);
    --accent: rgb(149, 175, 112);
    --accentlight: rgb(214, 241, 177);
    --accentdark: rgb(65, 86, 24);
    --bg: rgb(250, 252, 247);
    --bgdark: rgb(204, 223, 197);
    --bggrey: rgb(219, 230, 215);
    --bglightdark: rgb(233 241 233);
}

body {
    font-family: 'NanumSquareRound';
    background-color: var(--bg);
    color: var(--fg) !important;
}

a {
    color: var(--accent);
}

#blog-title {
    padding: 1rem;
}

#collection>nav {
    top: 5em !important;
    right: 1.5em;
    z-index: 99;
    width: 100px;
}

#collection>header {
    margin-top: 100px !important;
    display: flex;
    width: 100vw;
    max-width: 100%;
    padding: 0 !important;
    justify-content: space-between;
    flex-direction: column;
}

#collection>header>nav {
    display: flex !important;
    flex-wrap: wrap;
    width: 100vw;
    position: absolute;
    top: 0;
    left: 0;
    margin: 0 !important;
    justify-content: flex-end;
    align-items: center;
    max-width: 100vw;
    border-bottom: var(--bgdark) solid 1px;
    -moz-opacity: .4;
    -khtml-opacity: .4;
    -webkit-opacity: .4;
    opacity: .4;
    -ms-filter: progid:DXImageTransform.Microsoft.Alpha(opacity=40);
    filter: alpha(opacity = 40);
    -webkit-transition-property: opacity;
    -o-transition-property: opacity;
    transition-property: opacity;
    -moz-transition-duration: .4s;
    -webkit-transition-duration: .4s;
    -o-transition-duration: .4s;
    transition-duration: .4s;
}

#collection>header>nav>* {
    padding: 1em 2em;
    margin: 0 !important;
}

#collection>header>nav:hover {
    -moz-opacity: 1;
    -khtml-opacity: 1;
    -webkit-opacity: 1;
    opacity: 1;
}

#collection>header>nav>a:hover {
    text-decoration: none;
    background-color: var(--accent);
    color: white;
}

#collection>header>nav:before {
    content: " ";
}

.description.p-note:before {
    content: "- About -";
    display: block;
    color: var(--accent);
    margin-bottom: 20px;
}


.description.p-note {
    margin: 1em;
}

.p-author {
    font-family: 'Cafe24Shiningstar';
    color: var(--fg) !important;
}

.post-title, .post-title a {
    color: var(--accentdark) !important;
}

.font.norm, body#collection article.norm, body#post article.norm, body#subpage article.norm, input#title.norm, pre.norm, span.norm, textarea.norm {
    font-family: 'NanumSquareRound';
}

pre, code, textarea {
    font-family: 'intelone-mono-font-family-italic' !important;
}

footer > hr {
    display: none;
}

#wrapper {
    overflow: hidden;
    border-radius: 5px;
    max-width: 800px;
    border: var(--bgdark) 1px solid;
}

.norm.h-entry:last-of-type {
    border-bottom: 1px solid var(--bgdark);
}

.norm.h-entry:last-of-type .book.e-content {
    position:relative;
}

.norm.h-entry {
    margin: 0 !important;
    padding: 40px !important;
    background-color: white;
    max-width: 100% !important;
    border-bottom: var(--bgdark) 1px solid;
}

.norm.h-entry:hover {
    background-color: var(--bglightdark);
}

#post header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 !important;
    height: 4.4rem;
    border-bottom: 1px solid var(--bgdark);
    margin-bottom: 40px !important;
}

#post header>nav {
    line-height: 4.4em;
    display: flex;
    margin: 0 !important;
}

#post header>nav>* {
    padding: 0 2em;
    margin: 0 !important;
}

#post header>nav>a:hover {
    text-decoration: none;
    background-color: var(--accent);
    color: white;
}

body#post header nav a.pinned.selected, body#post header nav span.pinned.selected {
    font-weight: 400;
}

#post-body {
    border-radius: 5px;
    margin: 0 auto !important;
    max-width: 720px !important;
    border: var(--bgdark) 1px solid;
}

#post-body:hover {
    background-color: white !important;
}

.book.e-content>*:not(.link-and-banner) {
    display: none !important;
}

article:not(:last-of-type) .book.e-content .link-and-banner {
    display: none !important;
}

.link-and-banner {
    position: absolute;
    top: 300px;
    text-align: center;
    width: 100vw;
    max-width: 800px;
    left: -40px;
    margin-top: 40px;
    padding-top: 40px;
    padding-bottom: 40px;
    border-top: 1px solid var(--bgdark);
    background: var(--bg);
}

article:has(.link-and-banner:hover) {
    background-color: white !important;
}

.banner-code {
    max-width: 400px;
    margin: 0 auto;
    border: 1px solid var(--bgdark);
    font-size: 12px;
    text-align: left;
    border-radius: 5px;
    background: white;
}

#post .link-and-banner {
    display: none;
}

body#collection #paging, body#subpage #paging {
    overflow: visible;
    padding: 1em 6em 0;
    margin-bottom: 0 !important;
}

#emailsub {
    margin-top: 4em;
    margin-bottom: 500px;
}

@media (max-width: 700px){
    
    .p-author {
        font-weight: 400;
    }
    
    
    #collection>header>nav {
        flex-direction: column;
        height: 4.4em;
        max-width: 100vw !important;
    }

    #collection>header>nav:before {
        position: absolute;
        right: 0;
        top: 0;
        padding: 1rem;
        content: "\2630";
        font-size: 2em;
        width: 1.5em;
    }
    
    #collection>header>nav:hover {
        -moz-opacity: 1;
        -khtml-opacity: 1;
        -webkit-opacity: 1;
        opacity: 1;
        z-index: 999;
        background-color: var(--accent);
        max-width: calc(100vw - 120px) !important;
        right: 0;
        left: unset;
        height: 100dvh;
        justify-content: center;
        color: white;
        position: fixed;
    }
    
    #collection>header>nav:hover>a {
        display:block;
        color: white !important;
    }
    
    #collection>header>nav>a {
        display:none;
    }
    
    #post>header {
        margin-bottom: 0 !important;
        border-bottom: 1px solid var(--bgdark);
    }
    
    #post>header>nav:before {
        position: absolute;
        right: 0;
        top: 0;
        padding: 1rem;
        content: "\2630";
        font-size: 2em;
        width: 1.5em;
        line-height: 1em;
    }
    
    #post>header>nav:hover {
        display: flex;
        flex-direction: column;
        align-items: center;
        z-index: 999;
        background-color: var(--accent);
        max-width: calc(100vw - 120px) !important;
        width: 100%;
        top: 0;
        right: 0;
        margin-right: 0 !important;
        left: unset;
        height: 100dvh;
        justify-content: center;
        color: white;
        position: fixed;
    }
    
    #post>header>nav:hover>a {
        display:block;
        color: white !important;
    }
    
    #post>header>nav>a {
        display:none;
    }

    #post-body {
        padding: 40px 5px !important;
        border: 0px;
        border-bottom: 1px solid var(--bgdark);
    }
    
    .xtra-feature,span.views {
        display:none !important;
    }
    
}
```

# Post Signature

```
<div class="link-and-banner">
<h1>배너</h1>

<p><img src="(image url)"></p>
<p class="banner-code"><textarea><a href="(your blog url)"><img src="(image url)"></a></textarea></p>
</div>
```