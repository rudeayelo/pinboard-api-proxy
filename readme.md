# Pinboard API Proxy

> A CORS-enabled version of the Pinboard API

https://pinboard-api-proxy.now.sh

Use the information at https://pinboard.in/howto/#api to see what methods are available, just replace the domain.

## Example:

```
const getPosts = async (apiToken) => {
  const url = `https://pinboard-api-proxy.now.sh/posts/all?auth_token=${apiToken}&format=json`;
  const res = await fetch(url);
  const data = await res.json();

  return data;
}

getPosts([YOUR-API-TOKEN]) // Returns all posts
```

> Originally made by [ZΛNDΞR](https://github.com/mrmartineau/pinboard-api) by using [Micro](https://github.com/zeit/micro) & hosted on [now](https://zeit.co/now) by [zeit](https://zeit.co)
