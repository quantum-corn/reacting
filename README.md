# Reacting

## My journey of learning React

### Beginning

After I progressed considerably into JavaScript and also implemented some of it in my [site](https://brokenbricks.netlify.app), I had a feeling there was more to make great sites, such as [this](https://www.seanv.dev). After trying to dig around a bit I learnt that it was made out of React. After I digged further, I learned that React is a Javascript framework by Meta, the same company that runs Facebook. Say what you may about the platform or the company, the aesthetics and UI/UX are to die for. That is my goal here. What I also learned is that this framework is responsible to give the site an app-like feel, compared to the site-like feel of the past. So, I decided to learn React.

---

### First lessons

A google search and I found tons of resources. But 2 that stood out are:

- the official site of [ReactJS](https://www.reactjs.org)
- the book ['The Road to Learn React'](https://www.roadtoreact.com)

I generally prefer learning from a book over learning from videos, and the book was used as a reference in MIT. So I felt that it was genuinely good, so got the PDF. But before I started reading it, I also checked out the ReactJS official site. I learned there about some new things.

> - React works via **components**.
> - React components are Javascript functions that return markup code.
> - React components can be nested.
> - The markup returned by React is in JSX (something new to me for now), which is different from HTML.
> - React components are used as HTML-like tags with the difference being that React components names must start with Capital letters but HTML tags start with small letters
> - React doesn't explicitly tell how to implement CSS.

At this point I decided to stop and read the book and use the site only secondarily.

---

### The Inspiration

The book asked the readers to try teaching the material they learn as a learning exercise. It is a philosophy I believe in anyway so I decided to take the challenge up. The author said he will help promote such attempts, so perhaps this will become a blog that someone actually reads. I am unsure how to document the journey in text though. Typing out lectures will waste a lot of time. So the best idea I have now is to write my thoughts as a list of points.

---

### Standing Up Before We Walk

- The app-like interface that I mentioned before in contrast to the old-school site-like interface is called [SPA](https://en.wikipedia.org/wiki/single-page_application) - Single Page Application.
- React is a view library, in something called the '[MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller) - Model View Controller' - which means it allows to render components as viewable elements.

#### Requirements and Setup.

- The reader must know HTML, CSS, Javascript (I do check the box, perhaps barely though)
- An understanding of [API](https://www.robinwieruch.de/what-is-an-api-javascript/)
- I use a Linux machine.
- It comes with a terminal.
- I use VSCode for IDE.
- `node` and `npm` are needed
- I also use git & Github

#### `node` and `npm`

- Refer to the official website of [`node`](https://nodejs.org) for the relevant installation information. `npm` comes with `node`.
- Check your installation with the following commands (in terminal - I use '`$`' to indicate that the command is intended to be run on terminal)

    ```cli
    $node --version
    $npm --version
    ```

- The bare minimum familiarity with `npm`:
  
  - `$npm init -y` Here `npm` is the name of the executable (program) we are trying to call to. In other words, `npm` is the base command. `init` is the subcommand that we pass to `npm`. It tells `npm` what we want it to do. `-y` is a flag (because it starts with `-`). Flags are like further customization options for the main subcommand. `init` is used to initialize the directory where it is run, as a node project. `-y` tells `npm` to assume a `-y`es for all default options for parameters required to initialize. You can skip the flag if you want to do the inititalization manually step-by-step.
  - `$npm install -g --save-dev <packagename1> <packagename2>`
  
    `install` tells `npm` exactly what you would guess. `--save-dev` is also a flag. <font color="scarlet">The rule is : If the flag is just one character, use `-`, otherwise use `--`.</font> And then we have a ` ` (whitespace) separated list of `<packagenames>` we want to install. <font color="scarlet">You must know the package name exactly.</font> `-g` tells `npm` to `install` the given packages `-g`lobally meaning they will be accessible anywhere on your system. Not using this flag will `install` it in the directory where you run the command from. `--save-dev flag` tells `npm` that the package is to be noted separately as it is only used in the development cycle, for example, to test code, and will not be a part of the release or deployed versions of the code.
  - `$npm uninstall <packagename>` does exactly what you would guess.
  - `$npm install react` installs React in the working directory(directory where the command is run).
  - **Yarn** is an alternative to npm.

#### How to React?

There are many ways to use React.

- [CDN](https://en.wikipedia.org/wiki/content_delivery_network)(Content Delivery Network) - Accessing the `react.js` file which is what the React library is, from a remote server from within the code inside a `script` tag. It is required to use **React DOM** as well. It can be done the same way.
- Installing `react` and `react-dom` via `npm` into the project. Using this method means having to deal with **Babel** which makes converts JavaScript ES6 (newer version) and JSX (React syntax) into plain JavaScript, for greater compatibility.
- To avoid all the above complications, we can use [`create-react-app`](https://github.com/facebookincubator/create-react-app). It is beginner friendly and this book uses that.

#### `create-react-app`

- There's 2 ways to use it.
  - Install it using `$npm install -g create-react-app`. You can check your installation using `$create-react-app --version`. Lastly `$create-react-app <AppName>`
  - You can use `$npx create-react-app <AppName>`. `npx` is a tool that comes with `npm`. It avoids the step of installing packages and lets you run packages from npm directory without manually installing. <font color="scarlet">The package is still installed. Only you didn't have to bother about it.</font>. This is the preferred method as it always uses the latest version from the register.
- I am working along as I learn to I ran `$create-react-app first-reaction`. It automatically creates the app directory. Check it out [here](./first-reaction).

---

### Finally Walking

#### The First Steps


