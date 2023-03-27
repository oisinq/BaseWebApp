# Base Web App

Check it out at: https://base-web-app-oisinq.onrender.com/

### Phase 1: Base Web App
Mission- Get up and running with the Base Web App. Should be able to run locally and be deployed on Render.

##### 0. Before you get started:
- [ ] <a href="https://dashboard.render.com/register" target="_blank">Create Render.com account</a>
- [ ] <a href="https://github.com/join" target="_blank">Create Github account</a>
- [ ] <a href="https://help.github.com/articles/set-up-git/#setting-up-git" target="_blank">Download and install Git (github's command line tool)</a>
- [ ] <a href="https://nodejs.org/en/download/" target="_blank">Download and install Node.js</a>
- [ ] Download and install a text editor (I recommend <a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a>)

##### 1. Make a copy of my existing project on github by forking the project at https://github.com/oisinq/BaseWebApp
<img width="400" alt="github" src="https://cloud.githubusercontent.com/assets/17851174/25285298/b990a2ae-2687-11e7-845c-2673aa704689.png">

##### 2. Find and open your terminal
<img width="115" alt="screen shot 2017-04-21 at 11 43 48 am" src="https://cloud.githubusercontent.com/assets/17851174/25285319/ce48dafe-2687-11e7-9fba-3262f406235f.png">

*Note: on Windows, it might be called Git Shell or Git BASH.*

##### 3. Use the command line to navigate to your desktop (or any folder you want to store this project):
- `ls` lists all files in a directory. If you're on a PC, the command is `dir` instead.
```
	cd ~/Desktop
	ls
```
you should see all the items on your desktop displayed in text in the terminal like so:

![oct-12-2016 21-51-18](https://cloud.githubusercontent.com/assets/17851174/25285297/b97b3586-2687-11e7-8d0a-075baed899c4.gif)


##### 4. Clone the Repository
When you create (or in this case, fork) a repository on GitHub, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations. Use the command line to
 - (1) clone your project from Github onto your own computer, then
 - (2) navigate into the project and then
 - (3) list all the files in the project:

```
	git clone https://github.com/YourUserName/BaseWebApp.git
	cd BaseWebApp
	ls
```

##### 5. Install dependencies
Install the project’s dependencies using npm, a tool used to install any other projects your project needs in order to run locally. View the dependencies your app needs [here](https://github.com/oisinq/BaseWebApp/blob/master/package.json#L9).
```
	npm install
```

##### 6. Run the project on your machine (your local server)
```
	npm start
```

##### 7. View the project running locally
Open a browser and navigate to `localhost:5000`


##### 8. Make a change in the code and refresh the page running at `localhost:5000`
Open the project with VS Code or whichever text editor you installed. Make a change to your code (ex. In `index.ejs` change the header text) and refresh your web browser- you should see the change!

Ejs is a templating language that stands for embedded javascript. It's like HTML but with some special sauce mixed in so that you can add in a little javascript that gets compiled to HTML before it's send to the browser. We won't really be using it for anything other than HTML today though.

Few editors that you might find helpful:
* [Sublime Text](https://www.sublimetext.com/) - free to evaluate, but requires licence if you plan to use it every day
* [Atom](https://atom.io/) - completely free editor
* [Visual Studio Code](https://code.visualstudio.com/) - another free to use editor

In fact, any text editor will  work - if you have favourite one, please use it!

#### 9. Set up your project in Render.com
Go to https://dashboard.render.com/. After logging in, click the "New +" button at the top of the screen and select "Web Service".
<img width="1333" alt="Screenshot 2023-03-27 at 11 29 07" src="https://user-images.githubusercontent.com/5693967/227920169-3002cf88-b9bc-4b71-9e99-76db2601fd52.png">

On the right-hand side of the screen, under the GitHub heading click "Connect account" and log-in with your GitHub account from earlier.

Now you can see a list of all of your GitHub repos – click "Connect" for the BaseWebApp repo.
<img width="1218" alt="Screenshot 2023-03-27 at 11 31 43" src="https://user-images.githubusercontent.com/5693967/227920768-c33b0359-18bb-41ec-b4b4-db3af4c85ed2.png">

On the next screen, use the following settings:
* Name: Use something unique like base-web-app-YOUR_USERNAME_HERE. This will be used for your website URL
* Region: Pick Frankfurt, this will make your website quicker for European users
* Build command: Type in "npm install"
* Start command: Type in "node project/start.js"

_*We use automatic deploys at HubSpot - but ours go to a 'QA' or 'staging' site. Can you think of why we might do that? Ask a hubspotter near you what they think!_


##### 10. View your app live! (it might take a few seconds to finish deploying)
After a minute or so, your app should be deployed! The URL is based off of the name from the previous step. If you followed these instructions, your URL should be `https://base-web-app-YOUR_USERNAME_HERE.onrender.com/`

##### 11. Push that change to github (which automatically deploys on Render)
*If your server is still running from before (it probably is), you can press control + c to halt it

```
	git add .
	git commit -m “made my first change”
	git push origin master
```

##### 10. View your change live! (it might take a few seconds to finish deploying)
After a minute or so, your app should be deployed! The URL is based off of the name from the previous step. If you followed these instructions, your URL should be `https://base-web-app-YOUR_USERNAME_HERE.onrender.com/`


### Phase 2 - Continue to work off of ‘Hello World’

A few tips before you begin:
 - **Test often**- when you make a change, make sure it works. You don't want to add a bunch of stuff and spend tons of time tracking a little thing down.
 - **Google everything!** - Google is a developers best friend. I'm not joking. No one actually just _knows_ this stuff... you just get really good at knowing what to google and reading/incorporating the answers you find.
 - **Ask for help** - Everyone around you is dying to help you out! Don't be afraid to ask, no matter how silly you think your question is (because trust me, it's not).

 [Option 1 - Personal website](https://github.com/zsobin/PersonalWebApp): This is the easier option, using only HTML and CSS.

 [Option 2 - Incorporate a database](https://github.com/glanza/DatabaseWebApp): this is more challenging, and only recommended for attendees who are familiar with HTML, CSS and a little bit of javascript.

Step-by-step instructions for these can be found in the repo READMEs.




----------------------------------------------------------------------------------------------


### Other resources

Here are some external resources we've gathered to help you with further development.

**Git and GitHub tutorials**
Version control is an important tool for every developer, and git is the most popular one. Learn more [useful git commands](https://try.github.io/levels/1/challenges/1), discover [the branching]( https://learngitbranching.js.org/) and then check [how to use GitHub](https://guides.github.com/activities/hello-world/) for your own project.

**Web App tutorials (HTML, CSS, JavaScript)**
There are plenty of different and more comprehensive tutorials and online resources to learn HTML, CSS and JavaScript.


- FreeCode Camp interactive web development tutorial: https://www.freecodecamp.org/
- Khan Academy free html and css tutorial: https://khanacademy.org/computing/computer-programming/html-css
- Comprehensive web development tutorial/documentation by Mozilla: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web

- CSS visual guide: https://cssreference.io/
- Flexbox tutorial: http://flexboxfroggy.com/

- HTML cheatsheet: http://www.hostingreviewbox.com/html5-cheat-sheet/

**More Web App tutorials (FE frameworks)**
Once you have comfortability with JS, CSS and HTML, try out a frontend framework to take your skills to the next level.

- Learning React with create-react-app: https://medium.com/in-the-weeds/learning-react-with-create-react-app-part-1-a12e1833fdc

**Inspiration and problem solving**
To practice your problem solving skills and find some inspiration, please check the following pages:
- [StackOverflow](https://stackoverflow.com/) is a great place to ask any question (or search for it first, because it’s very likely that someone has already asked the same question and got an answer :))
- [Code Pen](https://codepen.io/) is a great source of inspiration with a lot of projects based on HTML, CSS and JavaScript
- [Dev.to](https://dev.to/) is a blog platform where you can find plenty of useful posts from other developers.
