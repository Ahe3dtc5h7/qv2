[![](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/Ahe3dtc5h7/qv2.git)

```js
addEventListener(
    "fetch",event => {
        let url=new URL(event.request.url);
        url.hostname="appname.herokuapp.com";
        let request=new Request(url,event.request);
        event. respondWith(
            fetch(request)
        )
    }
)
```