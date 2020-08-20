
FILE views/posts/new.html.erb   =>> input on line 11 contains the form_authenticity_token
    An authenticity token is stored in the session (where hackers can't get it) that's used to check when the form is submitted & throws an error if the token is missing or doesn't match
    Use the following code:         
        <input type="hidden" name="authenticity_token" value="<%= form_authenticity_token %>">


ORIGINAL FORM (views/posts/new.html.erb):
<form method="POST" action="<%= posts_path %>">
  <label>Post title:</label><br>
  <input type="text" id="post_title" name="post[title]"><br>
 
  <label>Post description:</label><br>
  <textarea id="post_description" name="post[description]"></textarea><br>
 
  
  <input type="hidden" name="authenticity_token" value="<%= form_authenticity_token %>">
  <input type="submit" value="Submit Post">
</form>
 










http://localhost:3000/posts         =>>     views/posts/index.html.erb

http://localhost:3000/posts/:id

http://localhost:3000/posts/new     =>>     views/posts/new.html.erb






