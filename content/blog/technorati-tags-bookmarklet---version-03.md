---
title: "Technorati Tags Bookmarklet - version 0.3"
date: 2006-08-10T13:35:32+0000
tags: ["Hacks"]
draft: false
---

Those who already know and use Technorati Tags Bookmarklet here is its latest version.

==================================================================

<code>javascript: ( function() {   /*     Technorati Tag Book Marklet 0.3     Created First By: Lorrell <http://lorelle.wordpress.com>     Last Modified By: Rakesh <http://rakeshkumar.wordpress.com>  */   var a='';   var t=prompt('Enter Tags separated by commas','');   if(!t) return;   var tr=t.split(',');   a+='<p><img id="technorati_img" src="http://rakeshkumar.wordpress.com/wp-content/uploads/2006/08/technorati.gif" alt="Technorati" /><strong>Technorati: </strong>';   for(var i=0;i<tr.length;i++)   {      tr[i]=tr[i].replace(/^\s+/,"");     tr[i]=tr[i].replace(/\s+$/,"");     var tag_text=tr[i];     tr[i]=tr[i].replace(/\s+/g,"+");     if(i > 0){     a+=', ';    }     a+='<a href='+unescape('%22')+'http://www.technorati.com/tag/'+tr[i]+unescape('%22')+' rel='+unescape('%22')+'tag'+unescape('%22')+'>'+tag_text+'</a>';   }   a+='</p>';  prompt('Copy this html code, Press OK, Then Paste into your blog entry:',a); } )()</code>
==================================================================

For others, technorati tags bookmarklet is a Firefox bookmarklet to tag ur blog posts. First created by <a href="http://lorelle.wordpress.com/2005/10/14/a-tagging-bookmarklet-for-wordpress-and-wordpresscom-users/">Lorelle</a> and later modified by <a href="http://freehogg.wordpress.com/2005/12/01/technorati-tags-bookmarklet/">freehogg</a>.

<strong>Whats New in this version:</strong>
1. Comma seperated tags.
2. Spaces are allowed inside tags, you dont need to use (+) anymore
3. Tag text is more presentable now. i.e. for a tag like "Hindi Movie", though the internal tag will be like "Hindi+Movie", but the link
will show it as "Hindi Movie" only

<strong>Questions:</strong>
<strong> Q1. How to create bookmarklet</strong>
Ans: Copy the above script and paste it to Firefox's address bar. Drag and drop it to bookmarks toolbar. Right click on it, go to properties and verify the location.
The location should contain the above script. Change the name to something related like "Technorati Bookmarklet".

<strong>Q2. How to use it?</strong>
Ans: Just click on the bookmark. A dialogue box will open. Enter your tags in it, seperated by commas. (spaces are allowed within tags). It generates
the html code for tags. Copy and paste it in your blog post.

<strong>Q3. Why Technorati Tags?</strong>
Ans: A simpler explantion is that it adds meaning to the information that you are providing (i.e. your post). Tags work both ways, it helps sites like Technorati
to organize the contents properly and on the other hands it increases your reach to a broader audience.

<strong>Q4. But wordpress already has Categories?</strong>
Ans: There is a conceptual difference between categories and and tags. Both do almost the same work, but categories are mostly like for your own benefit, while tags are for others. So the categories can be something like "Trip", while tags will have something like "Ooty", "Shimla" . Lorelle has a <a href="http://lorelle.wordpress.com/2005/09/09/categories-versus-tags-whats-the-difference-and-which-one/">nice article</a> on this

Please leave ur comments if you are using it.

<hr /><img src="https://rakeshkumar.wordpress.com/wp-content/uploads/2006/08/technorati.gif" alt="Technorati" /><strong>Technorati: </strong><a href="http://www.technorati.com/tag/Firefox" rel="tag">Firefox</a>, <a href="http://www.technorati.com/tag/Technorati" rel="tag">Technorati</a>, <a href="http://www.technorati.com/tag/Tags" rel="tag">Tags</a>, <a href="http://www.technorati.com/tag/Bookmarklet" rel="tag">Bookmarklet</a>