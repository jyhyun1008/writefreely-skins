# Custom CSS

```css
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@200&display=swap');

@font-face {
    font-family: 'default';
    src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/2404@1.0/Freesentation-2ExtraLight.woff2') format('woff2');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: 'default';
    src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/2404@1.0/Freesentation-7Bold.woff2') format('woff');
    font-weight: bold;
    font-style: normal;
}

/*about sidebar*/

article:first-of-type #right-button {
    display: flex !important;
    position: fixed;
    z-index: 99999;
    width: 4rem;
    height: 4rem;
    bottom: 20px;
    left: 20px;
    justify-content: center;
    align-items: center;
    background-color: #f5f8fb;
    border-radius: 50%;
    font-size: 2em;
}

article:first-of-type #left-nav {
    gap: 12px;
    width: 250px;
    height: 100dvh;
    background-color: #f5f8fb;
    position: fixed;
    top: 0;
    left: 0;
    display: flex !important;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    font-size: 1rem !important;
    line-height: 1.5 !important;
    border-right: 1px solid #c0c8cf33;
}

#left-nav a {
    color: inherit;
}

#left-nav a:hover {
    text-decoration: none;
}

body#collection nav#manage {
    z-index: 999999;
    position: fixed;
}

body {
    overscroll-behavior-x: none;
    margin-left: 250px;
}

img#avatar {
    aspect-ratio: 1 / 1;
    object-fit: cover;
    max-width: 150px !important;
    height: auto;
    border-radius: 50%;
    border: 5px solid white;
}

#upspace, #downspace {
    height: 50px;
}

#blog-info, #category-list, #profile {
    width: 90%;
    display: flex;
    flex-direction: column;
}

#left-nav #blogTitle, #left-nav #cateTitle {
    color: #446879;
    line-height: inherit !important;
    margin: 0.25em 0 !important;
}

.blogName {
    font-size: 0.8em;
    color: #446879;
}

#category-list .category {
    width: 100%;
}


#category-list .category .first {
    padding: 0.5em 0;
    border-radius: 20px;
}

#category-list .category:hover .first {
    background-color: #c0c8cf33;
}

#category-list .category {
    position: relative;
}

#category-list .category .second {
    display: none;
    position: absolute;
    bottom: -100px;
    left: 200px;
    padding: 10px;
    border-radius: 20px;
    border: 1px solid #c0c8cf33;
    background-color: white;
    width: 100%;
}

#category-list .category .second div {
    padding: 0.5em 0;
    border-radius: 20px;
}

#category-list .category:hover .second {
    display: block;
    width: 90%;
}

#category-list .second div:hover {
    background-color: #f5f8fb;
}

@media (max-width: 700px) {
    
    body {
        margin-left: 0;
    }
    
    article:first-of-type #left-nav {
        display: none !important;
    }
    
    article:first-of-type #right-button {
        display: flex !important;
    }
    
    article:first-of-type #right-button:hover #left-nav {
        display: flex !important;
    }
    
}

/*about content*/

body, body#collection nav#manage li a.write {
    font-family: "Noto Sans JP", 'default' !important;
}

.font.norm, body#collection article.norm, body#post article.norm, body#subpage article.norm, input#title.norm, pre.norm, span.norm, textarea.norm {
    font-family: "Noto Sans JP", 'default';
}

#blog-title {
    font-family: "Noto Sans JP", 'default';
    font-weight: bold;
}

#title, .post-title {
    font-family: "Noto Sans JP", 'default';
    font-weight: normal !important;
}

.book > *:not(p, blockquote:nth-of-type(1)) {
    display: none !important;
}

.book > p:not(:has(.thumbnail)) {
    display: none !important;
}

.book blockquote {
    border: 0 !important;
    margin: 0 !important;
    padding: 0 !important;
    color: inherit !important;
}

.book img {
    display: block !important;
    height: 200px;
    width: 100%;
    object-fit: cover;
    border-radius: 20px;
}

#post-body #title {
    margin-top: 50px !important;
    color: white;
    background: linear-gradient(90deg, black, transparent);
}

#post-body time {
    color: white !important;
    background: linear-gradient(90deg, black, transparent);
}

#post-body .thumbnail{
    position: absolute;
    height: 180px;
    top: 70px;
    left: 0;
    object-fit: cover;
    width: 100vw;
    filter: brightness(50%);
    z-index: -1;
}

#post-body > .e-content > blockquote:nth-of-type(1) {
    padding-top: 50px;
    padding-bottom: 10px;
    position: relative;
    top: -80px;
    margin-bottom: -80px;
    z-index: -2;
    display: block !important;
    border-bottom: 2px solid #ddd;
    border-right: 2px solid #ddd;
    border-left: 2px solid #ddd !important;
    border-radius: 0 0 20px 20px;
}
```

# Post Signature

```
<div id="right-button" ><div>+</div><div id="left-nav"><div id="upspace"></div><a href="(Your Blog URL)"><img src="(Avatar URL)" id="avatar"/></a><div id="blog-info"><h2 id="blogTitle"><a href="(Your Blog URL)">여행당일기</a></h2><div id="blogDesc">잡다한 블로그</div></div><div id="category-list"><h2 id="cateTitle">카테고리</h2><div class="category"><div class="first">메인</div><div class="second"><a href="(Your Blog URL)"><div><b>전체보기</b></div></a><a href="(Your Blog URL)/category1"><div>Category1</div></a></div></div><div class="category"><div class="first">Next Blog</div></a><div class="second"><a href="(Your Next Blog URL)"><div><b>전체보기</b></div></a><a href="(Your Next Blog URL)/tag:category2"><div>Category2</div></a></div></div></div><div id="profile"><div class="blogName">(Your Namme)</div><div class="blogName"><a href="mailto:(Your Email)">Mail</a> · <a href="(Your Github Link)">Github</a> · <a href="(Your ActivityPub Link)">Misskey/Mastodon</a></div></div><div id="downspace"></div></div></div>
```