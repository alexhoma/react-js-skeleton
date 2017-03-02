# React JS Boilerplate

Single page app using React JS + Redux. It also comes with Babel ES6 compiler, React Router, SASS loaders and a very basic directory structure following the redux pattern.

It's basically a boilerplate to initialize my react.js projects.
Based on several resources.

## Initialize

Just type this commands to initialize the app:
```avascript
> npm install
> npm start
```

## Content
This boilerplate contains a blog view example with some posts related by categories.
No CRUD functionality added yet, it is just a view app.

The example data comes from a mock endpoint. Using [mockable.io](https://www.mockable.io).
Once you recieve the data, the post object looks like the following:

```javascript
{
    "id": 1,
    "slug": "hello-react",
    "title": "Hello React",
    "content": "The path of the righteous man is beset on all sides by the iniquities...",
    "author": "Samuel L. Jackson",
    "categories": [
        {
             "slug":"programming",
             "title": "Programming"
        },
        {
             "slug":"sports",
             "title": "Sports"
        }
    ]
}
```

## Deploy to Heroku
An easy way to check your app up and running is to deploy using heroku.

// tell heroku you are creating a new app (without the curly braces!)
> heroku create {your-app-name}
// check if your app runs well locally
> heroku local web
// push it to heroku
> git add .
> git commit -m "Deploying app"
> git push heroku master
// scale your web container to 1
> heroku ps:scale web=1
// open browser with your app
> heroku open