# blog-project
A blog

**Challenge 1:**
To complete challenge 1, you should be able to head over to localhost:3000 and when you hit enter it should render the home page and it will have an h1 but just says Home.

So in your home.ejs you'll need to create an h1 that says Home and by writing some code inside app.js, you should be able to get this to show up on localhost:3000.

**Challenge 2:**
In the app.js file, there are three of constants at the top:

const homeStartingContent = 
const aboutContent = 
const contactContent =

They just contain a whole bunch of Lorem Ipsum and randomly generated text.

Let's say that this the content that's in our server and we want to be able to deliver it over to our home page using EJS.

For this challenge have the home page display a "home" title using a h1 tag and the homeStartingContent inside a paragraph tag.

On your browser, when you go to localhost:3000 you will see an h1 that says home, but also the same text that's held inside that constant which is homeStartingContent.

**Challenge 3:**
Inside the home.ejs file there is an HTML boilerplate and a title.

In this challenge, replace the header and footer layout partials inside the respective header.ejs and a footer.ejs files.

When you refresh your website you should see the nav bar,

the three links in the nav bar, a brand on the left and a footer at the bottom with some text. And you'll

see all of the CSS that we've got inside our styles.css being applied to this web page.

**Challenge 4:**
Inside the project, in the views folder, create a new folder called partials.

Inside this folder drag the header and footer.ejs files.

When you come across Node Express EJS apps, there are main web pages and then there are our partially complete HTML files inside a folder called partials. This is usually the structure that you will see. 

To complete this challenge try and fix the code so that your header and footer partials still get

applied.

**Challenge 5:** 
Now in this challenge in order to complete it, go into your browser and go to

localhost:3000/about and be able to see the about page with the same header and footer and CSS

applied to this page. And also to be able to go over to the contact page and again have this page rendered

with a header and footer using the partials and also have the data that's inside the app.js,

about content and contact content rendered and passed over to the correct pages.

**Challenge 6:** Update the code so that when you click on these the nav bar links (home, about us, contact, us) in the nav bar they actually take us to the correct pages.

So when you click on about, it should go to the About page and contact goes to a contact page. The challenging part is is figuring out where to change this code.

**Challenge 7:**
The goal of this challenge is to be able to head over to the path that's localhost:3000

/compose and be able to render a page that has the same styling as the rest of the pages with

our nav bar and our footer and to have an h1 that says compose as the title of the page. And then we're going to have a text input and button that has the text publish.

**Challenge 8:**
The goals for this challenge is to update the code so that when we go over to our compose page and we type something and we click publish then we should see that blog entry immediately in our console.

**Challenge 9:**
Create a compose form with bootstrap enabled on a title input and a post input.

The title input is a single line and the post input is a multi line text box 

You also need to make this publish button blue and look like this.

We've got some extra labels in hand above the title and post input boxes.

**Challenge 10:**
Currently there are two inputs inside our form. One is called post body and one is called post title. 

Inside our app.js we currently can console.log the post title that gets sent to our compose route through the post requests that the form initiates.

So when we click the submit button we send over two pieces of data, the textarea and the input.

The next challenge is instead of console logging the post body or the post title inside this callback, create a Javascript object that's simply just called post and it has to store both the title that gets passed over as well as the post body that gets passed over.

**Challenge 11:**
In this challenge put this newly created post object inside a global variable called

posts, with an 's' at the end.

We're going to have an array that is going to store all of these new posts but it's going to be a global variable.

You need to create a new empty array that is a global variable and then you're going to add this new post object to that new array.

And finally at the end of this route, you're going to redirect to the root route. And inside the root route we're going to log all of the posts inside the post array that you created.

Once you've completed this, what should happen is I should be able to put in a post hit publish

and then let's go back to compose again and let's put in another post and hit publish.

And firstly you notice that we get directed to the root route or the home page

once we've finished composing the post. And then if you take a look inside our terminal you can see that

my entire array is being logged and the first time it only contained a single object, the 'Day 1 post, and the second time this array

contained two Javascript objects both of my posts, 'Day 1' and 'Day 2'.

**Challenge 12:** 
Instead of console logging the posts, pass them over to the home.ejs page and console.log the posts array there.

**Challenge 13:**
Write a FOR loop inside the home.ejs page that loops through the post array and console logs each and every title, the titles of each of these posts. And to test it you should have a minimum of two posts so that you can make sure that you are indeed printing out all of the titles inside the posts array.