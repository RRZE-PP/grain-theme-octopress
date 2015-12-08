---
layout: post
title: "Post sample with code"
date: "2000-01-01 00:01"
author: SysGears + RRZE P&P
categories: [grain, groovy]
comments: false                    # disables/enables comments section for the post
published: false                   # defines whether to render the post in 'generate' mode
sharing: true                     # (optional) disables/enables sharing options for the post, 'true' is by default
asides: [ ]              # (optional) asides to include into the post page, all asides are included by default
---

<!--more-->

##Example with line numbers:

####Code:

&#096;&#096;&#096;groovy HelloWorld.groovy<br>
println "Hello, world!"<br>
&#096;&#096;&#096;

####Result:

```groovy HelloWorld.groovy
println "Hello, world!"
```

##Example without line numbers:

####Code:

&#096;&#096;&#096;groovy**:nl** HelloWorld.groovy<br>
println "Hello, world!"<br>
&#096;&#096;&#096;

####Result:

```groovy:nl HelloWorld.groovy
println "Hello, world!"
```

------

## jsFiddle tag

####Code:

```jsp
<%= jsfiddle shorttag: '8wcwq', width: '90%', skin: 'light', tabs: 'html,css,js,result' %>
```

####Result:

<%= jsfiddle shorttag: '8wcwq', width: '90%', skin: 'light', tabs: 'html,css,js,result' %>

------

## Gist tag

####Code:

```jsp
<%=
    gist id: 'dc3bf4796acd6a1439bc'
%>
```

####Result:

<%=
    gist id: 'dc3bf4796acd6a1439bc'
%>

------

## HTML5 Video tag


####Code:

```jsp
<%=
    video urls: [
        'http://html5demos.com/assets/dizzy.mp4',
        'http://html5demos.com/assets/dizzy.webm',
        'http://html5demos.com/assets/dizzy.ogv'
    ]
%>
```

####Result:

<%=
    video urls: [
        'http://html5demos.com/assets/dizzy.mp4',
        'http://html5demos.com/assets/dizzy.webm',
        'http://html5demos.com/assets/dizzy.ogv'
    ]
%>

------

##Image tag

Note, that theme `img` tag can handle all the attributes of standard HTML 'img' tag, such as align, border, etc.

##Link to the internal image:

####Code:

```jsp
<%= img src: '/images/email.png', alt: 'email image' %>
```

####Result:

<%= img src: '/images/email.png', alt: 'email image' %>

##Link to the external image:

####Code:

```jsp
<%= img src: 'http://cdn1.sysgears.com/images/grain/logo-cacd6d0f221a8f8cab3c46db5b0e730a.png', height: 100, width: 200 %>
```

####Result:

<%= img src: 'http://cdn1.sysgears.com/images/grain/logo-cacd6d0f221a8f8cab3c46db5b0e730a.png', height: 100, width: 200 %>

------

##Raw tag

Raw tag is used here to prevent groovy code parsing.

####Code:

```jsp
<%= raw text: '${ 2 + 2 }' %> = ${ 2 + 2 }
```

####Result:

<%= raw text: '${ 2 + 2 }' %> = ${ 2 + 2 }

------

##Pullquote tag

##Right-aligned Quote

####Code:

```jsp
<%= pullquote content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. {/Ut enim ad minim veniam/}. Quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
qui officia deserunt mollit anim id est laborum.'''
%>
```

####Result:

<%= pullquote content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. {/Ut enim ad minim veniam/}. Quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
qui officia deserunt mollit anim id est laborum.'''
%>

##Left-aligned Quote

####Code:

```jsp
<%= pullquote align: 'left', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. {/Ut enim ad minim veniam/}. Quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
qui officia deserunt mollit anim id est laborum.'''
%>
```

####Result:

<%= pullquote align: 'left', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. {/Ut enim ad minim veniam/}. Quis nostrud exercitation ullamco
laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa
qui officia deserunt mollit anim id est laborum.'''
%>

------

##Blockqoute tag


####Code:

```jsp
<%= blockquote content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>
```

####Result:

<%= blockquote content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>

##Quote from a printed work

####Code:

```jsp
<%= blockquote author: 'John Doe', sourceTitle: 'Lorem ipsum', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>
```

####Result:

<%= blockquote author: 'John Doe', sourceTitle: 'Lorem ipsum', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>

##Quote from Twitter

####Code:

```jsp
<%= blockquote author: 'John Doe', sourceLink: 'http://example.com', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>
```

####Result:

<%= blockquote author: 'John Doe', sourceLink: 'http://example.com', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>

##Quote from a post

####Code:

```jsp
<%= blockquote author: 'John Doe', sourceTitle: 'Lorem ipsum', sourceLink: 'http://example.com', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>
```

####Result:

<%= blockquote author: 'John Doe', sourceTitle: 'Lorem ipsum', sourceLink: 'http://example.com', content:
'''Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua.'''
%>

------

