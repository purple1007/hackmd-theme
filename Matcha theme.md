---
description: 
- Add `{%hackmd SJVxgnJbp %}`。
- Add `{%hackmd @debbylin/theme-matcha %}` 即可套上樣式
---

<style>
    /*   Colors   */
    body {
        --text-primary: #80986a;
        --bg-color: #f6f4f1;
        
        --bg-gray: #efedea;
        --bg-gray-dark: #ebe9e4;
        
        --bg-lighter-blue: #dfe5eb;
        --border-blue: #7095d8;
        
        --bg-light-yellow: #f0e7cf;
        --text-yellow: #dba614;
        
        --bg-light-green: #eaf4e6;
        --text-green: #5CB85C;
        
        --bg-light-red: #f1dddd;
        --text-red: #d07070;
        
    }
    
    /*   Docs background color   */
    #meta-title-tags {
        background-color: none;
    }
    
    body, .ui-content,
    #doc.markdown-body, 
    .ui-view-area, 
    .ui-comment-app .open-comments, 
    #meta-title-tags > .w-full {
        background-color: var(--bg-color) !important;
    }
    
    /*   Headline  */
    .markdown-body h1,
    .markdown-body h2 {
        border-bottom: 1px solid #dcdad8;
    }

    .markdown-body h1, .markdown-body h2,
    .markdown-body h3 {
        color: var(--text-primary);
    }
    
    /*   Image   */   
    .markdown-body img, .markdown-body iframe {
        border: 1px solid rgba(0, 0, 0, 0.1);
        margin: 0.5rem 0rem;
        border-radius: 0.6rem;
    }
    
    .markdown-body img.emoji {
        border: none;
        width: 20px;
        height: 20px;
        vertical-align: middle;
    }
    
    /*   iframe  */
    .markdown-body ifame, 
    .markdown-body embed {
       max-width: 100%;
       width: 728px;
       border-radius: 0.6rem;
       overflow: hidden;
    }
    
    /*   Spoiler   */
    .markdown-body details {
        padding: 0.5rem 1rem;
        background-color:  var(--bg-gray);
        margin-bottom: 0.5rem;
        border-radius: 3px;
    }
    .markdown-body details:hover {
        background: var(--bg-gray-dark);
        transition: .1s all;
    }
    .markdown-body details[open]:hover {
        background-color:  var(--bg-gray);
    }
    .markdown-body details summary {
        cursor: pointer;
    }
    .markdown-body details summary + p {
        margin-top: 0.5rem;
    }
    .markdown-body details code {
        background-color: var(--bg-gray-dark);
    }
    .markdown-body details p:last-child {
        margin-bottom: 0px;
    }
    
    /*   Alert  */
    .markdown-body div.alert {
        border: none;
        border-radius: 0.5rem;
    }
    
    .markdown-body div.alert h2,
    .markdown-body div.alert h3,
    .markdown-body div.alert h4,
    .markdown-body div.alert h5,
    .markdown-body div.alert h6 {
        margin-top: 0px;
    }
    
    /*   info block  */
    .markdown-body div.alert.alert-info {
        color: inherit;
        background-color: var(--bg-lighter-blue);
        border-left: 3px solid var(--border-blue);
    }
    
    /*   warning block  */
    .markdown-body div.alert.alert-warning {
        color: var(--text-yellow);
        background-color: var(--bg-light-yellow);
        border-left: 3px solid var(--text-yellow);
    }
    
    /*   success block  */
    .markdown-body div.alert.alert-success {
        color:  var(--text-primary);
        background-color: #e0e9d9;
        border-left: 3px solid var(--text-primary);
    }
    
    /*   danger block  */
    .markdown-body div.alert.alert-danger {
        color: var(--text-red);
        background-color: var(--bg-light-red);
        border-left: 3px solid var(--text-red);
    }
    
    
    /*   Date and comment  */
    .markdown-body li small,
    .markdown-body blockquote .small,
    .markdown-body blockquote small {
        font-size: 85%;
        display: initial;
    }
    
    .markdown-body .mark, 
    .markdown-body mark {
        color: var(--text-yellow);
        background-color: var(--bg-light-yellow);
        border-radius: 3px;
    }
    
    /*   code block   */
    .markdown-body code, 
    .markdown-body tt,
    .markdown-body:not(.next-editor) pre {
        background-color:  var(--bg-gray);
        border-radius:  0.6rem;
        overflow:  hidden;
    }
    
    /*   Link   */
    .markdown-body a {
        color: var(--text-primary);
    }
    
    /*  Table  */
    .markdown-body table th {
        background-color: var(--bg-gray);
    }
    .markdown-body table td {
        background-color: var(--bg-color);
    }
    
    /*   hr   */
    .markdown-body hr {
        height: 3px;
        background-color: var(--text-primary);
        border-radius: 10rem;
        overflow: hidden;
    }
</style>
