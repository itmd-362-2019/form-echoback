## Setup

1. Clone the repository (duh).
2. Change into its directory (`cd form-echoback`)
3. Install the dependencies: `npm install`

## Use

Out of the box, you can test the default form in `public/index.html` by running:

    $ npm start

And going to `http://localhost:3000` in your web browser. Fill out the values, and hit the submit
button. You'll get a JSON representation echoing the data that the server received via a POST
request.

To test your own form, just copy it into the `public/` directory, overwriting `index.html` if you’d
like. Set your form’s `action` attribute to `/process-data` and the `method` attribute to `post`,
something like this:

```html
<form id="signup" action="/process-data" method="post">
```
