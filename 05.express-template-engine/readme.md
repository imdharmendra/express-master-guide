# Template Engine

**A template engine enables you to use static template files in your application. At runtime, the template engine replaces variables in a template file with actual values, and transforms the template into an HTML file sent to the client. This approach makes it easier to design an HTML page.**

## Template Engine

- pugjs :  https://pugjs.org/api/getting-started.html

- handlebars : https://www.npmjs.com/package/handlebars

- ejs : https://www.npmjs.com/package/ejs

## Setup ejs on express project

```
app.set('view engine','ejs');

res.render("home",{title:"Home Page"})

```

## EJS Template Tag Syntax

- <% %>

- <%= %>

- <%- %>

- <%# %>

- <%  -%>

- <%_ %>

- <%  _%>

## Hello with EJS

```
<h1> <%= title %></h1>
```

## Control Statement in EJS

```
<% if(title) { %>
  <h1> <%= title %></h1>
<% } %>


<% if(title) { %>
  <h1> <%= title %></h1>
<% } else { %>
  <h1> <%= title %></h1>
<% } %>
```

## Loope with ejs Example

```
<ul>
  <% for(let i=1;i<=5;i++) { %>
    <li>Item <% = i %> </li>
  <% } %>
</ul>
```

## Array loop with EJS

```
<% let items=["a","b","c",'d'] %>

<ul>
  <% items.forEach(item=>{ %>
    <li>Item <% = item %> </li>
  <% }) %>
</ul>

```

## Template Partials (Part)

```
<%- include('header') -%>

```



















