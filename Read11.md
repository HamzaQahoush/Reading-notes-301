### Whats is EJS 

EJS is a template system.  we define HTML pages in the EJS syntax and we specify where various data will go in the page. Then, 
our app combines data with the template and "renders" a complete HTML page where EJS takes our data and inserts it into 
the web page according to how you've defined the template. For example, we could have a table of dynamic data from a database 
and we want EJS to generate the table of data according in our display rules. It saves us from the drudgery of writing code to 
dynamically generate HTML 
based on data.

EJS is compatible with Express for back-end use as it hooks into the View engine architecture that Express provides and lets you render web pages to the  the client with `res.render()` in Express.


### Basic Syntax(Tags):

`<% 'Scriptlet' tag, for control-flow, no output`

`<%= Outputs the value into the template (HTML escaped)`

`<%- Outputs the unescaped value into the template`

### Example

`<% if (message) { %>`

  `<h2><%= message.name %></h2>`
  
`<% } %>`
