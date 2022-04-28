# 🚀 Getting Started

## What's inside? 🧐

* Headless [WordPress](https://wordpress.org/) via [WPGraphQL](https://www.wpgraphql.com/)
* [Next.js](https://nextjs.org/)
* [Sass](https://sass-lang.com/)
* [Cloudinary](https://cloudinary.com/)
* Deployed to [Netlify](https://netlify.com/)


### Requirements
* [WordPress](https://wordpress.org/)
* [WPGraphQL](https://www.wpgraphql.com/)
* Environment variables (see below)


Add an `.env.local` file to the root with the following:
```
WORDPRESS_GRAPHQL_ENDPOINT="http://wordpressite.com/graphql"
```


### Environment

This project makes use of WPGraphQL to query WordPress with GraphQL. In order to make that request to the appropriate endpoint, we need to set a environment variable to let Next.js know where to request the site information from.

Create a new file locally called `.env.local` and add the following:

```bash
WORDPRESS_GRAPHQL_ENDPOINT="[WPGraphQL Endpoint]"
```

Replace the contents of the variable with your WPGraphQL endpoint. By default, it should resemble `[Your Host]/graphql`.

*Note: environment variables can optionally be statically configured in next.config.js*

#### All Environment Variables

| Name                               | Required | Default | Description                                       |
| ---------------------------------- | -------- | -       | ------------------------------------------------- |
| WORDPRESS_GRAPHQL_ENDPOINT         | Yes      | -       | WordPress WPGraphQL endpoint (ex: host.com/graphl)|
| WORDPRESS_MENU_LOCATION_NAVIGATION | No       | PRIMARY | Configures header navigation Menu Location        |
| WORDPRESS_PLUGIN_SEO               | No       | false   | Enables SEO plugin support (true, false)          |

### Development

To start the project locally, run:

```bash
yarn dev
# or
npm run dev
```

The project should now be available at [http://localhost:3000](http://localhost:3000)!


