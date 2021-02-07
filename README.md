# welcome

Dear Coder, thank you so much for becoming a part of the Webhikers team and joining our journey to deliver better websites and webapps to the world:)

It's our goal to be working with you in the long run and providing you with new jobs on a daily basis. So, please give this `readme` a quick shot.

- [Intro](#intro)
- [The Product](#product)
- [The Procedure](#procedure)
- [Guidelines](#guidelines)
- [Closing](#closing)

<a name="product"/>

## The Product

We are creating [headless websites](https://blog.cpanel.com/how-to-use-wordpress-as-a-headless-cms/) and webapps for our clients, using `WordPress` as a `headless CMS` for the backend and `Vue.js` or `Nuxt.js` as the frontend.

- `simple websites` will be created directly with `Nuxt.js` 
- `webshops` will be created in `Vue.js`, so we can implement the `Vue.js` components into our own `core`.

We will take care of the `design` and the `backend`, so you only need to bother with the frontend.

You will receive 2 things from us:

1. an `adobe XD design` to convert it into `Vue.js` code for the frontend. 
2. the required information to fetch data from the server into your `frontend application`.

Along the way, there's a few things you need to know and that you have to take care of:

<a name="procedure"/>

## The Procedure

1. We will send you an adobe XD File, which needs to be converted to a `Vue.js` or `Nuxt.js` app.
2. While you convert the XD file to code, we will prepare a `headless` WordPress site and fill it with content.
3. As soon as you finished the conversion from `XD` to `code`, you will receive a file with the following information.
  - the `baseURL` for the `REST API`
  - the `page_ids` for all pages
  - custom `post_type` names if there are any
  - A `google recaptcha site key`, if there is a form on the page
  - A `form_id` if there is a form on the page
  - A list with all `form inputs` that are accpted by the server for each form

<a name="guidelines"/>

## Coding Guidelines

It's very important to learn a few of our simple coding practices, so your code alignes well with ours:

### 1. The architecture

**(read `before` you convert the XD file to code)**

File organization, naming conventions and scoping is extremely important to build maintainable websites and webapps. Sometimes we will merge your code with some code of ours and sometimes you will create standalone websites. However, if you stick to the following rules, you will write perfectly organized webapps, that we can work with. Don't worry, it's not that many rules, most of them are self-explanatory and best-practices anyway.

[Please read this little info tutorial once and apply it to all projects that you're doing for us.](https://github.com/Webhikers-Docs/code-architecture)

If you have any questions, please contact me ANYTIME at christian@webhikers.at.

### 2. Installation of `bootstrap-vue` in `Nuxt.js` projects

**(read `before` you convert the XD file to code)**

I've received projects, where the `bootstrap-vue` `scss source` has been imported into every single component, resulting in a giant compiled css file, where the bootstrap source has been included several times.

If you're perfectly confident, that you're importing and using `bootstrap-vue` correctly, then you can skip this step. [Otherwise, please shortly walk with me through the installation process](https://github.com/Webhikers-Docs/nuxt-bootstrap-doc), to install `bootstrap-vue` the correct way.

### 3. Fetching Data from our clients `WordPress` sites

**(read `after` you convert the XD file to code)**

This is just a short documentation with a little `api helper script`. Here you can find the REST API endpoints for `pages`, `posts` and `custom_post_types`. Since the WordPress REST API, doesn't send the response UTF-8 decoded, we need to decode the response manually. This is what our `api helper script` is doing. If you have a better alternative, you don't have to stick with this script.

You can find the documentation [here](https://github.com/Webhikers-Docs/wp-api-doc)

### 4. Submitting a form to Wordpress

**(read `after` you convert the XD file to code)**

1. We will create a form in WordPress (Contact Form 7 Plugin) and define all accepted input fields manually. For example: `fullname`, `email`, `message`.
2. We will send you the `field names` in a seperate file with all other project related data.
3. You will create the frontend form and submit `fullname`, `email`, `message` to the clients WordPress site.

Please use [this very short documentation](https://github.com/Webhikers-Docs/bootstrap-vue-cf7) to build forms in our projects

<a name="closing"/>

## Closing

I know, that seems like quiet a bit of information, but most of this is self-explanatory and you can always come back to find a specific info. Also you will be able to remember all guidelines very fast as soon as you start to implement them.

We do value your time, your effort and your work a lot. If there is something we can improve, please let us know and if there is something you don't understand, please ask as often as you need to. Please also remember that "stupid questions" **do not** exist.

For coding related questions you can always reach me at christian@webhikers.at.

Thank you so much for reading and **happy coding** :)
