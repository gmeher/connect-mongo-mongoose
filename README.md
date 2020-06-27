# 1. Belb
This application looks pretty much the same like the original [Yelp](https://www.yelp.com) website.

It leverages the free [Yelp Fusion REST API](https://www.yelp.com/developers/documentation/v3) for which you need an API key.

1. Head over to the [Yelp Fusion API documentation](https://www.yelp.com/developers/documentation/v3)
2. Click on `Create App` and sign in if you haven't done so already
3. Once you have signed in, click on the `Get Started` button. If you already have an app, then you will already see the API key
4. Fill out the form for [creating a new app]
5. Copy the generated `API key`  that must be put inside the header of each request
6. Navigate to the `src/hooks/yelp-api/config.js` file and assign the `BEARER_TOKEN` variable the following content
   ```
   const BEARER_TOKEN = '<your-token-here>'
   ```
7. Install the dependencies by running `npm install` or `yarn install`
8. Run the app with `npm start` or `yarn start`


# 2. Used Technologies
* [React / create-react-app]
    * **only functional components**
    * communication with web servers with [React Hooks] only
    * no higher order or class-based components
* [React router] with [useReactRouter]
* [Bulma]
* Flexbox