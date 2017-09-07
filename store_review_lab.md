# Comic Book Store Reviews Lab (for learning VueJS)

## Objectives
This lab will take students generally through converting a simple reviewing application (which does not use any sort of Javascript) to one that uses Vue.JS to add, modify, and remove content on the fly. The goals for this lab are to:

1. Introduce students to the Vue.JS framework and basic Vue.JS syntax.
2. Give students an experience adding dynamic front-end effects to a completed web application.
3. Introduce general techniques for debugging Vue.JS.
4. Walk students through adding dynamic feedback to showcase front-end changes.
5. Help students identify opportunities to add dynamic effects to applications.

### Part 1: Introduction to Vue.JS
While students will certainly have a chance to learn the basics of Vue.JS through an introductory lecture, perhaps it is worth preparing a brief recap of Vue.JS?

Regardless, it should be worth noting the documentation for Vue.JS can be found [here](https://vuejs.org/v2/guide/).

### Part 2: Walking Through the Reviewing Application Front-End
Here, we will introduce students to the reviewing application as-is. The application is a general Rails application which acts as a review board for local Comic Book shops in Pittsburgh. 

**Note that at this point the reviewing application is a relatively barebones Rails application** (with minimal CSS to help students focus on the content, informational flow, and UX).

The following functionalities would be supported:
1. Adding new shops to review.
2. Adding reviews to existing shops (starts and description).
3. Editing reviews to existing shops.
4. Removing reviews to existing shops.

For the sake of the lab, let's assume there are no user accounts supported in the application, so anyone can modify anyone else's material.

We will have students walk through the existing application by having them perform several operations through the front-end, such as: 

## Checkpoint 1
The TAs will look to see that the students have:
1. Gotten the Rails 5 application up and running.
2. Added a new shop to be reviewed 
3. Added a new review to this shop as themselves.
4. Deleted an existing review.

### Part 3: Identifying Slowdowns and Pain Points of the Reviewing Application
Here, students will have an opportunity to explore the existing (static) functionality of the reviewing application in order to identify areas of improvement using Vue.JS.

This section will walk through why browser refreshes hinder the experience of using the reviewing application for relatively quick sections of the application, including:
1. Adding a new post.
2. Editing an existing post.
3. Removing a post.
(Note: I propose leaving out adding a store using Vue as another exercise due to time constraints).

### Part 4: Adding a Review in Vue
This is the first part of the lab in which students will modify the existing experience of adding a review of a store (which exists by redirecting to another page) to run through Vue without redirecting screens.

Students will have to save the review using Rails/Vue to the DB.

The goals of this section are:
1. To convert an existing HTML form to be run through Vue.
2. To get experience saving data through Vue.
3. To consider ripple effects of modifying aggregate data (changing overall store rating on the fly)

## Checkpoint 2
The TAs will look to see that the students have:
1. Modified the form so that no new page is rendered at any step of adding a review.
2. Created a form which dynamically updates the front-end upon creating a review (have them post a review).
3. Posted new reviews so that they are indeed saved to the database (refresh the page).
4. Adding a new review changes other data on the page (such as average review).

### Part 5: Editing and Deleting Reviews
Building off being able to add a review using Vue, this portion of the lab will walk students through editing and removing reviews using Vue as to improve the user experience. This section will be pretty similar to adding a new review where they will either remove a post or provide the ability to edit a post right on the page.

## Checkpoint 3
The TAs will look to see that the students have:
1. Modified the form so that no new page is rendered at any step of editing or deleting a review.
2. Created a form which dynamically updates the front-end upon editing a review (have them edit a review).
3. Posted changed reviews so that they are indeed saved to the database (refresh the page).
4. Editing/deleting a review changes other data on the page (such as average review).
5. Deleting a review works as expected without any page re-rendering.

## Bonus Material
Upon completing the lab, students can work on adding a new store for review using Vue.
