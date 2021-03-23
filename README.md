### Run locally (default: `localhost:1313`)
```
./localserver
```

### Publish Instructions
```
./publish
cf push
```

### Add New Recipe
```
hugo new recipes/(title).md
```

## Disable Home Page Icon
To disable the homepage and remove icon from sidebar, set the `noHomeIcon` param in `/config.toml`:

``` toml
[params]
noHomeIcon = false
```

## Redirect to Different URL
To redirect to the `/recipes` route by default, uncomment the following in `/layouts/partials/index.html`:
``` html
<meta http-equiv="refresh" content="0; url=/recipes" />
```
