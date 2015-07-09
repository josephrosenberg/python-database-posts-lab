# Python Database Blog Posts Lab

## Concept

This lab will help you create your own Blog backend! After this lab you will be able to write simple posts and store them in between visits to your blog.

## Objectives

+ Create a blog post database model
+ Make a corresponding frontend that allows users to create posts
+ Show a list of all posts

## Directions

1. Fill in the `Post(ndb.Model)` with a `StringProperty` for a title, a `TextProperty` for the content, and a `DateTimeProperty` that automatically records the date the record was created.
2. Fill in the `get()` of `MainHandler` so it queries for all the posts and sends it to the template to render
  + It might be good to just print the values to the console or send the raw text with `self.response.write` until you flesh out the frontend
3. Build up the frontend HTML so it can display all the posts.
4. Add a form to the front end that posts to the `/` root url with a new title and content for a post.
5. Fill in a `post()` method in `MainHandler` that gets the data from the form, creates a new `Post`, and stores it in the datastore.

## Stretch

+ Use the Users api to replace the person posting with the signed in Users
+ Make the site look better with CSS and more creative HTML
+ Validate content and user name.
+ Add an email field
