# `gatsby-source-local-meetups`

Pulls data about upcoming events in a given category for a specific area.

## Example

In your `gatsby-config.js`
```js
module.exports = {
  plugins: [
    {
      resolve: "gatsby-source-local-meetups",
      options: {
        // get this at https://secure.meetup.com/meetup_api/key/  
        apiKey: 'your_api_key',
        category: 'tech',
        latitude: '29.4241',
        longitude: '-98.4936',
        maxEvents: 10, // optional, default: 20
      }
    }
  ],
}
```