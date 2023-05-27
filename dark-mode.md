---
title: Editor - Dark - CSS - Basic (default font)
tags: style, CSS
description: Add {%hackmd @debbylin/editor-dark-bacis %} in your HackMD note
---

{%hackmd @debbylin/colors %}
{%hackmd @debbylin/docs-render-dark %}

<style>
/*  Editor color  */
    .ui-edit-area.unselectable.ui-resizable,
    .cm-s-one-dark.CodeMirror, 
    .cm-s-one-dark .CodeMirror-gutters,
    .cm-s-one-dark .CodeMirror-scroll {
        background-color:  var(--zinc-900);
        color: var(--zinc-300);
    }
    
    .CodeMirror-lines {
        padding: 8px 0;
    }
    
    .CodeMirror pre.CodeMirror-line, 
    .CodeMirror pre.CodeMirror-line-like {
        padding-right: 1rem;
        padding-left: 0.4rem;
    }
	
    .CodeMirror-overlayscroll-horizontal div, 
    .CodeMirror-overlayscroll-vertical div {
        border: none;
    }
    
/*  editor-basic  */
    .cm-s-one-dark .cm-string-2,
    .cm-s-one-dark .cm-variable-2,
    .CodeMirror-foldmarker,
    .cm-s-one-dark .cm-string,
    span.cm-m-markdown,
    .cm-s-one-dark .cm-variable-3{
        color: var(--zinc-300);
    }
    
/*  editor-comment   */
    .cm-s-one-dark .CodeMirror-foldgutter-open:after,
    .cm-s-one-dark .cm-string,
    .cm-s-one-dark .cm-comment,
    .cm-s-one-dark .CodeMirror-guttermarker-subtle,
    .cm-s-one-dark .CodeMirror-gutter-elt,
    .cm-s-one-dark .cm-def,
   .cm-s-one-dark .cm-quote {
        color: var(--zinc-400);
    }
    
/*  editor-mark  */
    .cm-s-one-dark .attribute,
    .cm-s-one-dark .cm-number,
    .cm-s-one-dark .cm-qualifier,
    .cm-s-one-dark .cm-plus {
        color: var(--zinc-300);
    }
    
/*  editor-Primary-color  */
    .cm-s-one-dark .cm-hr,
    .cm-s-one-dark .cm-variable,
    .cm-s-one-dark .cm-link,
    .cm-s-one-dark .cm-property,
    .cm-s-one-dark .cm-m-markdown.cm-keyword,
    .cm-s-one-dark .cm-m-markdown.cm-tag,
    .cm-s-one-dark .cm-m-markdown.cm-builtin,
    .cm-s-one-dark .cm-atom {
          color: var(--primary-400);
    }
    
    .cm-s-one-dark .CodeMirror-foldmarker, 
    .cm-s-one-dark .CodeMirror-foldgutter-folded:after {
          color: var(--primary-400) !important;
    }
    
    .cm-s-one-dark .CodeMirror-cursor {
        border-left: 2px solid var(--primary-600) !important;
    }
    
/*  editor-headline-color  */
    .cm-s-one-dark .cm-header,
    .cm-s-one-dark .cm-string-2 {
        color: var(--primary-400);
    }
    
   /*  editor-red  */
    .cm-s-one-dark .cm-operator,
    .cm-s-one-dark .cm-bracket {
        color: var(--red-500);
    }
    
/*  editor-blue  */
    .cm-s-one-dark .cm-meta {
        color: var(--sky-600);
    }
    
/* editor-error */
    .cm-s-one-dark .cm-spell-error,
    .cm-s-one-dark .cm-minus,
    .cm-s-one-dark .cm-error {
        color: var(--pink-300);
    }
    
    .cm-indent-guide {
        border-color: var(--zinc-700);
    }
    
/*   line number   */
    .cm-s-one-dark .CodeMirror-linenumber {
        color: var(--zinc-700);
		display: none;
    }
    .cm-s-one-dark.CodeMirror-focused .CodeMirror-activeline .CodeMirror-gutter-elt {
        color: var(--zinc-600);
    }
    
/*  editor - selected  */ 
    .CodeMirror-gutter-background,
    .cm-s-one-dark.CodeMirror .CodeMirror-selected,
    .cm-s-one-dark .CodeMirror-activeline-background {
        background: var(--zinc-800) !important;
        opacity: 0.7;
    }
    
/*   search bar  */
    .CodeMirror-dialog-top {
        border: none;
        top: 0;
        background-color: var(--zinc-800);
    }
    
/*   search result   */
    .cm-searching {
        background-color: var(--primary-500);
        color: var(--zinc-200) !important;
    }

    .cm-matchhighlight {
        border-bottom: none;
        background-color: var(--zinc-700); 
    }

    .authorship-gutter {
        opacity: 0.2;
    }
    
/*  the editor max width  */   
    .ui-edit-area.unselectable.ui-resizable {
            max-width: 700px;
            margin: auto;
    }
	
	
/*   the sorllbar of edior   */
    .CodeMirror-overlayscroll-vertical {
        width: 8px;
    }
    .CodeMirror-overlayscroll-horizontal div, 
    .CodeMirror-overlayscroll-vertical div {
        background-color: var(--zinc-700);
    }
	
 /* scorll connect */
    .ui-edit-area .ui-resizable-handle.ui-resizable-e {
        background-color: var(--zinc-900);
        width: 8px;
        right: -8px;
        box-shadow: none;
        transition: all 0.03s;
        border-left: 2px solid var(--zinc-800);
    }
    .ui-edit-area .ui-resizable-handle.ui-resizable-e:hover {
        background-color: var(--zinc-900);
        border-left: 2px solid var(--zinc-700);
    }
    
    .ui-toc.both-mode {
        margin-left: 2px;
    }
    
    .ui-edit-area button.ui-sync-toggle {
            left: calc(50% - 4px);
    }
    button.ui-sync-toggle.btn-default {
        color: var(--zinc-400);
        background-color: var(--zinc-700);
        border: none;
        box-shadow: none;
    }
    button.ui-sync-toggle.btn-default:hover {
        color: var(--zinc-300);
        background-color: var(--zinc-600);
    }

    
     /*  當編輯是雙欄模式時不限制寬度  */   
    .ui-edit-area.unselectable.ui-resizable.col-lg-6 {
        max-width:  initial;
    }
    .row.ui-content {
        background-color: var(--zinc-900); 
    }
    
    /*  tool  bar */
    .tool-bar  {
        background: var(--zinc-900);
        border-bottom:  1px solid var(--zinc-700);
        color: var(--zinc-400);
        font-size: 14px;
        height: 38px;
    }
    .tool-bar a {
        color: var(--zinc-400) !important;
        width: 23px;
        height: 23px;
    }
    .tool-bar i.separator {
        border-left: 1px solid var(--zinc-800);
    }
    .tool-bar a.active, .tool-bar a:hover {
        background-color: var(--zinc-700);
        border: none;
        color: var(--zinc-300) !important;
    }
    
    /*  status-bar    */
    .status-bar .status-indicators,
    .status-bar, 
    .status-bar .status-info,
    .status-bar .status-indicators .status-keymap>a,
    .status-bar .status-indicators .status-theme>a,
    .status-bar .status-indicators .status-spellcheck>a, 
    .status-bar .status-indicators .status-breaks>a,
    .status-bar .status-indicators .status-linter>a, 
    .status-bar .status-indicators .status-preferences>a
     {
        background: var(--zinc-900);
        color: var(--zinc-500);
        opacity: 1;
    }
    .status-bar .status-indicators .status-keymap>a:hover,
    .status-bar .status-indicators .status-theme>a:hover,
    .status-bar .status-indicators .status-spellcheck>a:hover, 
    .status-bar .status-indicators .status-breaks>a:hover,
    .status-bar .status-indicators .status-linter>a:hover, 
    .status-bar .status-indicators .status-preferences>a:hover
    .status-bar a:hover {
        color: var(--zinc-300) !important ;
    }
    .status-indicators .status-length {
        color: var(--zinc-500) !important;
    }
    .status-bar .status-indicators>div {
        border-left-color: var(--zinc-700);
    }
    .status-bar {
        border-top-color: var(--zinc-700);
    }
    
    /*  navbar & like & bookmark */     
    .navbar-default, 
    .btn-default {
	    background-color: var(--zinc-900);
  	    border: none;
        color: var(--zinc-500);
    }
    
    .btn-default.active, 
    .open>.dropdown-toggle.btn-default {
        color: var(--zinc-100);
        background-color: var(--zinc-900) ;
    }
    
    .ui-infobar .btn.btn-default,
    .ui-comment-app .open-comments .btn.ui-open-comments {
        border: 1px solid var(--zinc-700);
        color: var(--zinc-500);
    }
    
    .community-button,
    .navbar-default .navbar-nav>li>a,
    .navbar-right .btn.ui-status.online {
        color: var(--zinc-500);
    }
    
    .community-button:hover,
    .btn-default:hover,
    .btn-default.active.focus, 
    .btn-default.active:focus, 
    .btn-default.active:hover, 
    .btn-default:active.focus, 
    .btn-default:active:focus,
    .btn-default:active:hover, 
    .open>.dropdown-toggle.btn-default.focus,
    .open>.dropdown-toggle.btn-default:focus, 
    .open>.dropdown-toggle.btn-default:hover,
    .navbar-default .navbar-nav>.open>a, 
    .navbar-default .navbar-nav>.open>a:focus, 
    .navbar-default .navbar-nav>.open>a:hover,
    .navbar-default .navbar-nav>li>a:focus,
    .navbar-default .navbar-nav>li>a:hover,
    .navbar-right .ui-menu:hover {
        color: var(--zinc-300) !important;
        background-color: var(--zinc-800) !important;
    }
	
	
    /*  dropdown menu  */
      .dropdown-menu>li>a {
          color: var(--zinc-500);
      }
     .dropdown-menu {
          background-color: var(--zinc-800);
		 font-family: 
            'Inter', -apple-system, BlinkMacSystemFont,
            "Segoe UI", "Helvetica Neue", Helvetica, Roboto,
            Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
      }
	
	.divider {
		border-bottom: 1px solid var(--zinc-700);
	}
	.dropdown-menu .divider, 
	.input-group .input-group-btn .ui-share-copy:hover,
	.input-group .input-group-btn .ui-share-copy:focus,
	.permission-dropdown .ui-share-preview:hover,
	.permission-dropdown .ui-share-preview:focus,
	.menuitem-dropdown .menuitem-dropdown-trigger:hover, 
	.menuitem-dropdown .menuitem-dropdown-trigger:focus,
	.dropdown-menu>li>a:focus, 
	.dropdown-menu>li>a:hover { 
		color: var(--zinc-300);
		background-color: var(--zinc-700);
    }
	.form-control,
	.input-group .input-group-btn .ui-share-copy,
	.permission-dropdown .ui-share-preview,
	.menuitem-dropdown .menuitem-dropdown-trigger {
		  border: 1px solid var(--zinc-600);
		  background-color: var(--zinc-800);
		  color: var(--zinc-400);
	}
	
	.menuitem-dropdown .dropdown-menu .menuitem-item.disabled {
		color: var(--zinc-600);
	}
	
	/* 	input */	
	.form-control:focus {
		border: 1px solid var(--zinc-400);
		background-color: var(--zinc-900);
		box-shadow: none;
	}
	
	/* 	navbar buttons */
	.navbar-right .btn.ui-status.online:hover,
	.navbar-right .btn.ui-status.online:focus,
	.navbar-right .ui-host-list.open .btn.ui-status.online,
	.menuitem-dropdown .menuitem-dropdown-trigger:hover, 
	.menuitem-dropdown .menuitem-dropdown-trigger:focus {
		 background-color: var(--zinc-700);
	}
	.navbar-right .btn.ui-sharing.signin,
	.navbar-right .ui-share-button.open .btn.ui-sharing.signin,
	.btn-primary {
		color: white;
		background-color: var(--primary-600);
		border: none;
	}
	.navbar-right .btn.ui-sharing.signin:hover,
	.navbar-right .btn.ui-sharing.signin:focus,
	.btn-primary:hover, .btn-primary:focus {
		color: white;
		background-color: var(--primary-700);
		border: none;
	}
	
	.permission-dropdown .ui-more-settings, 
	.permission-dropdown .sidenav-trigger,
	.public-publish-container a {
		color: var(--primary-400);
	}
	
   /*    TOC   */  
    /*      unselected   */    
    .ui-toc-dropdown .nav>li>a {
        color: var(--zinc-500);
    }
    /*     selected   */   
    .ui-toc-dropdown .nav>li>a:focus,
    .ui-toc-dropdown .nav>li>a:hover,
    .ui-toc-dropdown .nav>.active:focus>a, 
    .ui-toc-dropdown .nav>.active:hover>a,
    .ui-toc-dropdown .nav>.active>a {
        color: var(--zinc-300);
        border-left-color: var(--zinc-300);
    }
  
/*  TOC button in both mode */
    .expand-toggle,
    .back-to-top, .go-to-bottom  {
        color: var(--zinc-500);
    }
	.expand-toggle:hover, .expand-toggle:focus, 
	.back-to-top:hover, .back-to-top:focus,
	.go-to-bottom:hover, .go-to-bottom:focus {
		color: var(--primary-400);
	}
    .ui-toc-label:focus {
          background-color: var(--zinc-700);
          color: var(--zinc-300);
      }

 /*   Comment   */
    .ui-comment-app .ui-comment-button {
        color: var(--zinc-500);
    }
    .ui-comment-app .ui-comment-button-container.comment.active:not(.simple),
    .ui-comment-app .open-comments {
        background-color: var(--zinc-900);
    }
    
    .ui-comment-app .open-comments .btn.ui-open-comments.open,
    .ui-comment-app .open-comments .btn.ui-open-comments.open:focus { 
        background-color: var(--zinc-900);
        color: var(--zinc-500);
        border: 1px solid var(--zinc-700);
    }
    
    .ui-comment-container {
        background-color: var(--zinc-900);
        border: 1px solid var(--zinc-700);
    }
    
    .ui-comment-container textarea {
        color: var(--zinc-300);
        border: 1px solid var(--zinc-700);
        background-color: var(--zinc-900);
    }
    
    .ui-comment-container.highlighted {
        background-color: var(--zinc-850);
    }
    
    .ui-comment-container .ui-comments-container .ui-comment .comment-author, 
    .ui-comment-container .ui-comments-container .ui-comment .comment-content
	{	
		color: var(--zinc-300); 
	}
    a.view-comments {
        color: var(--primary-400);
    }
    
</style>