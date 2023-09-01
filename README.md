# Flask-Based-Post-Updated
Building upon previous foundation, I've recently upgraded my skills to include the development of a RESTful blog.

# What I Have Learned and Upgraded Skills
Through this project, I embarked on a journey of Flask web development and Bootstrap styling. Initially, I created a user-friendly website with various routes to handle different pages – the main page, about page, individual blog posts, and a contact page. Leveraging the Jinja templating engine, I dynamically rendered HTML templates and displayed blog posts retrieved from an external API.

To enhance the visual appeal and responsiveness of the application, I harnessed the power of Bootstrap's CSS framework. This provided me with pre-designed components and responsive layouts, ensuring that the website looked great on a wide range of devices. I even incorporated FontAwesome icons to add an extra layer of visual aesthetics.

One of the project highlights was the contact page, which allowed users to get in touch by submitting a form. I skillfully handled form submissions using Flask's request object and integrated email functionality via the smtplib library. This feature enabled the seamless sending of emails to a designated recipient, complete with the submitted contact information.

# Upgrading Skills to a RESTful Blog
I've recently upgraded my skills to include the development of a RESTful blog. This enhancement allows for more advanced interactions with the application. I've implemented the principles of REST (Representational State Transfer) to create a robust API for the blog. This means users can now perform CRUD (Create, Read, Update, Delete) operations on blog posts programmatically, opening up exciting possibilities for automation and integration.

This project showcases my evolving expertise in Flask web development, routing and URL handling, HTML templating with Jinja, making HTTP requests, handling form submissions, and integrating email functionality. Moreover, with the addition of RESTful capabilities, it demonstrates my commitment to staying current in web development trends and technologies.

You can explore the source code for this project on my GitHub repository, which serves as a testament to my practical experience and proficiency in web development, encompassing Flask, Bootstrap, and now RESTful APIs. My journey in web development continues, and I look forward to new challenges and opportunities for growth.

## Step 1: Setting Up the Basics
I kicked off the project by creating a Flask web application. Flask is a Python web framework that makes it simple to build web applications. In the beginning, I imported essential modules like Flask, render_template for rendering HTML templates, redirect and url_for for navigation, and more.

## Step 2: Managing Styling with Bootstrap
To make my application visually appealing and responsive, I utilized Bootstrap, a popular front-end framework. It helps ensure that the user interface looks great on various devices and screen sizes.

## Step 3: Database Connection
For storing and retrieving blog posts, I integrated a SQLite database using flask_sqlalchemy. This allowed me to create a BlogPost class as a model to define the structure of a blog post, including the title, subtitle, date, content, author, and image URL.

## Step 4: Creating Blog Posts
To provide an intuitive way to create blog posts, I implemented the CreatePostForm class using FlaskForm. This form contains fields for the title, subtitle, author, image URL, and the main content of the blog post. The CKEditorField from the flask_ckeditor library enabled a rich text editing experience.
![create post button](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/334398df-0b1d-4a4e-9fb3-d44c33ff2042)
![create-new-post](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/6299bb64-6faa-48a8-9d64-1df3462fc332)
![post saved succesfully](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/ab40a0fb-e4f3-4198-8f77-473bd2c0e82c)

## Step 5: Displaying Blog Posts
To display all existing blog posts, I set up a route that queries the database for all posts using BlogPost.query.all(). These posts are then sent to the index.html template, where they're rendered dynamically. Each blog post's title, subtitle, and a brief preview are shown.
![get_all_posts](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/96454991-2e48-46a3-a49a-8b3346ef9cfb)

## Step 6: Viewing Individual Posts
When a user clicks on a specific blog post, the application uses the show_post route to retrieve the post's details from the database and render them using the post.html template. This page displays the complete content of the selected post.
![individual-post](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/9ed9e9b0-88c1-452d-af22-ab0fa8d18821)

## Step 7: Editing and Deleting Posts
Enabling editing and deleting functionality was crucial. The edit_post route allows users to modify the content of an existing post, while the delete_post route lets them remove a post from the database.
![edit-post](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/c7c5bb45-2578-49f1-913d-4d9c70982b8c)
![delete-post](https://github.com/teodoraspirovska/Flask-Based-Post-Updated/assets/133661233/cd602263-8d3f-448d-8080-c2dda2ea2181)

## Step 8: About and Contact Pages
I also included "About" and "Contact" pages using the respective routes. These pages provide users with additional information about the website and a way to get in touch.

## Step 9: Deployment
Once everything was ready, I was able to run the application locally using the if __name__ == "__main__" block. You can adjust the host and port settings based on your preferences. To take it a step further, you could deploy the app to a web server to make it accessible to a wider audience.

# The Result: Flask Blog CMS
And there you have it! My Flask Blog CMS is a user-friendly platform that empowers you to write, edit, and manage your blog posts effortlessly. With the use of Flask, SQLAlchemy, Bootstrap, and other libraries, I've created a seamless experience for both bloggers and readers. Whether you're just starting out or you're an experienced blogger, this CMS provides all the tools you need to share your thoughts with the world.

