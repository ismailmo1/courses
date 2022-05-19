# Web Dev Resources

My first run in with web technologies was when I was looking for ways to share python scripts with colleagues at work - exe files generated with tools like py2exe kept getting blocked by IT so I knew there had to be a better way.

I searched for courses on udemy and found a course and jumped straight in. It really opened up the world of software engineering and made a lot of concepts click - I just wish I discovered it earlier!

## Courses

<details>
<summary><b>Colt Steele's Web Developer Bootcamp</b></summary>

[Udemy Course Link](https://www.udemy.com/course/the-web-developer-bootcamp/)
|
[Final Project Repo](https://github.com/ismailmo1/yelpCamp)
|
[Final Project Hosted Website](https://yelpcamp.ismailmo.com/)

<p>This was the first course I took on anything web development related and at this stage I didn't realise that I could use my existing knowledge with a web framework in python.</p>

It was a blessing in disguise though since I ended up learning Javascript in this course where I developed a standard CRUD app with an ExpressJS (nodeJS) backend.

Stuff I learnt:

- HTML, CSS, Javascript
- MongoDB
- ExpressJS, NodeJS
- Bootstrap
- General web development concepts:
  - APIs
  - frontend <-> backend integration
  - ORMs
  - npm

</details>

<details>
<summary><b>Corey Schafer's Flask Series</b></summary>

[Youtube Playlist Link](https://www.youtube.com/watch?v=MwZwr5Tvyxo&list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)

<p> I should probably keep this to myself, but after taking the course on web dev using nodeJS as a backend I still felt like javascript didn't give me everything I needed and I still wanted to do some things (mostly data stuff) in python.

I remember googling how to run python processes in nodeJS and luckily I somehow stumbled across Corey's videos on the [Flask](https://flask.palletsprojects.com/) web framework and that really brought it all together.

I had built up a decent foundation from the udemy course: I had the basic understanding of how a web server worked, the request - response cycle and connecting to a DB etc. so this playlist of videos was more than enough to get me going with a proper project: [Formpy](https://github.com/ismailmo1/formpy-app)

</p>
(New) Stuff I learnt:

- Flask
- Best practices
  - refactoring
  - design patterns
- Virtual environments
- Deployment

</details>

<details>
<summary><b>Building Formpy</b></summary>

[Formpy-app Repo](https://github.com/ismailmo1/formpy-app)
|
[Formpy Repo](https://github.com/ismailmo1/formpy)
|
[Formpy Hosted Website](https://formpy.ismailmo.com/)

<p>If there's one piece of advice that gets repeated in the "self taught programming" circles, it is to stop doing so many tutorials and start learning by building projects.

That's solid advice and I would repeat that advice to my old self or anyone that would listen, but it's really tough to scope out a project thats big and complex enough to be interesting, but small and simple enough to be feasible for someone whose word count in google search comfortably beats that in VSCode during a typical coding session.

Building Formpy was a super long and drawn out project, but I'm really proud of what I built. At it's core - its simply a openCV based program that read's multiple choice forms like [scantron](https://www.google.com/search?tbm=isch&as_q=scantron). The real satisdaction is that anyone can use it, and it solves a real problem from end to end (see the repo for details).

I refactored this project more times than I can recall (you can check the git history if you're really bored), and I learnt how to deploy on a vanilla linux server with docker. I also ended up separating the code into two different repos: one for the web app and the other for the core functionality which I released as a python package with docs and CI/CD!

[formpy-omr package](https://pypi.org/project/formpy-omr/) |
[formpy-omr readthedocs site](https://formpy.readthedocs.org/)

</p>

</details>

<details>
<summary><b>Academind's React - Complete Guide</b></summary>

[Udemy Course Link](https://www.udemy.com/course/react-the-complete-guide-incl-redux/)

<p>

Building formpy was a huge lesson on how difficult it can be to build UIs in a imperative manner with vanilla javascript. If you look at the [javascript source code](https://github.com/ismailmo1/formpy-app/tree/master/app/app/static/scripts) for formpy (sorry) you will experience some of the pain I did with the number of
`document.createElement`s scattered everywhere. Of course there was a better way.

I was deep enough into the web dev world where I knew of web frameworks like React so I first tried reading through the [React docs](https://reactjs.org/docs/getting-started.html) (they're fantastic btw) but I realised that I prefer learning initially through video courses and then using docs as a reference, so I found Maxmilian's course and got stuck in.</p>

Stuff I learnt (and built):

- Modern Javascript
- React Basics - JSX/Components
- Hooks, Context API ([Food Order App](https://github.com/ismailmo1/shopping-UI))
- Redux
- JWT Authentication ([firebase based auth](https://github.com/ismailmo1/react-auth/))
- React Router ([Single Page App](https://github.com/ismailmo1/react-quotes))
- Typescript with React ([React Typescript](https://github.com/ismailmo1/react.ts))
- Meta-frameworks: NextJS ([Meetups App](https://github.com/ismailmo1/nextjs-meetups))

I then built a [Football Draw Simulator](https://github.com/ismailmo1/ucl-draw) ([live website](https://ucl-draw.web.app/)) to flex the new skills.

</details>

## What's next?

As I work my way through more courses, I try and push the bar higher to justify sitting through a new course. I feel like I have enough fundamental knowledge now so I try stop myself from going through another course and try jump into projects more with the confidence that I will learn what I need when I need it, and focus more on implementing good design patterns and learning stronger software engineering principles.

I'm currently building [family-tree](https://github.com/ismailmo1/family-tree) which uses FastAPI (python) as a backend and NextJS (typescript) as a frontend and hope to keep building things and my expertise.
