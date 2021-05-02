Partials
Partials are templates that we can write, that we can include in other templates. For example our html boilerplate, we don’t want to include on every template, that’s not very DRY.

Partials File Structure
Because partials are still templates, we are going to include them in the views folder, in their own sub-directory.

![](https://i.ibb.co/VqvS91w/partilas.png )
Linking Partials in Templates
`<% include templateName %>`
