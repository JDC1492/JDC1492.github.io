---
layout: post
title:      "On and Off the Rails"
date:       2020-11-08 17:50:11 +0000
permalink:  on_and_off_the_rails
---


Ruby on rails was the focus for the past three weeks. This was a challenge for myself for a couple of reasons. One reason, in particular,  was because I found it difficult to understand the often celebrated 'magic' of the framework. Leading up to this section I grew accustomed to doing alot of the groud work on my own. Form helpers  in rails are a great example of that.  In the previous section of sinatra, writing out our forms consited of HTML tags, Input and label tags with the need of having to have made sure that the appropriate tags recieved thier proper closing tags as well. 

```
<form method="post" action="/games">
<input type="text" name="titlle" >
<input type="text" name="genre" >
<input type="submit" value="Create Game">
</form>

```

 In the basic example above the form takes in the name and the genre of a new game into the database. Notice that it accepts a method and an action in the opening form HTML tag. As devs we know that upon the creating/submitting of the new game that this will send a post http request to the index page of our web application, through the action giving our post request a "goal".

Alot of work(basic example in this case), but work that I was used to. 

Rails makes life easier with form helpers.  

```
<%= form_with model: @game, local: true do |f| %>
<%= f.text_field :title %>
<%= f.text_field :genre %>
<%= f.submit %>
```

With no method or action telling ths button where to submit being declared on our end 'explicitly',  the 'magic' being performed on the back end looks more like:

```
<form action=”/games” accept-charset=”UTF-8" method=”post” data-remote=”true”>
 <input name=”utf8" type=”hidden” value=”✓”>
 <input type=”hidden” name=”authenticity_token” value=”…”>
 <input type=”text” name=”game[title]”>
 <input type=”text” name=”game[genre]”>
 <input type=”submit” name=”commit” value=”Create” data-disable-with=”Create”>
</form>
```

Comparing the actual work against the form helper syntax, its safe to say that form helpers are very useful and time savers. Rails is filled with things that help speed up your processes in the beginning stages of your web-application from generating resources, models and even a full app with scaffold.  This level of abstraction for devs is appreciated and I look forward to getting more knowledge of both the complex and simple within this language of Ruby.

