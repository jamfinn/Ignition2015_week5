#### Deliverables for week 5 Rails MVC
##### Odin Project Routing Guide Questions:
- **What is the "Root" route?**  
-This is the route to bring the user to whatever the homepage is, making it the default url.  It's key! 

- **What are the seven RESTful routes for a resource?**  
- GET all the posts (aka "index" the posts)
GET just one specific post (aka "show" that post)
GET the page that lets you create a new post (aka view the "new" post page)
POST the data you just filled out for a new post back to the server so it can create that post (aka "create" the post)
GET the page that lets you edit an existing post (aka view the "edit" post page)
PUT the data you just filled out to edit the post back to the server so it can actually perform the update (aka "update" the post)
DELETE one specific post by sending a delete request to the server (aka "destroy" the post)

- Which RESTful routes share the same URL but use different verbs?
- Get '/posts' and Post '/posts'
- Get '/posts/:id' , Put '/posts/:id' and Delete '.posts/:id'

- How do you specify an ID or other variable in a route?
-':id' tells rails to find and save this id in the params hast.  This way you can do multiple GEt requests for many posts and save them to the same route. 

- How can you easily write all seven RESTful routes in Rails?
-'resources :posts' in config/routes.rb

- What is the Rails helper method that creates the HTML for links?
- '_path' and '_url' at the end of methods will create HTML links. 

##### Odin Project Views Guide Questions:
- What is a layout?
- This is a basic view layout that will be used in all of your pages, so it has the javascript and css needed already loaded.  This makes the views simpler, easier  to load.
- 
- What's the difference between a "view template" and a "layout"?
- The layout is just a shell with the css and javascript needed, whereas the view template actually has the html needed across all pages.

- What is a "Preprocessor"?
- A preporocessor loads the html, css, and javascript for a view into on singular file before it is submitted to the view.  This makes it easier and faster to load.
- 
- Why are preprocessors useful?
- see above
- 
- How do you make sure a preprocessor runs on your file?
-you make sure the file has html.erb, or whichever correct file extension.  Rails will process the file with the outside extensions, working in to convert them into the next inner language.  Rails comes with most preporcessors installed.

- What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file?
-html;css 

- What is the difference between the <%= and <% tags?
- <%= will output the Ruby output of this code, while <% will just run the code, without dispaying the output.
- 
- What is a view partial?
- This is a template that can be reused within views so that a view doesn't have to be repeated.
- 
- How do you insert a partial into your view?
- To insert a partial, you first create the partial, denoted by an underscore, then use the render method to insert it into the view.
-
- How can you tell that a view file is a partial?
- It starts with an underscore.
- 
- How do you pass a local variable to a partial?
- You can create an new object and refer to a variable in the parent view to pass a local variable into the partial. "partial:"
- 
- What's the magical Rails shortcut for rendering a User? A bunch of Users?
- To render 1 user,  you can create a lop to create and render a user from the @users collection.  To render many, you can call do "render @users" and rails will run this loop over the entire users collection.

- What are asset tags and why are they used?
- Asset tags are used to identify CSS or Javascript files so that they can be outputted and identiied when compiled into one html file for the view. 

##### Link to Odin Project Basic Routes, Views and Controllers repo: [my odin repo](<linkhere>)
##### Link to Hartl's Rails Tutorial Chapter 5 repo: [my hartl's repo](<linkhere>)
