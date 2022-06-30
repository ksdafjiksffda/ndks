[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/apps
template=https://github.com/ksdafjiksffda/ndks.git)

```
addEventListener(
  "fetch", event => {
    let url = new URL(event.request.url);
    url.host = "appname.herokuapp.com";
    let request = new Request(url, event.request);
    event.respondWith(
      fetch(request)
    )
  }
)
```
