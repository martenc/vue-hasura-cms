# blog-app

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn run serve
```

### Compiles and minifies for production
```
yarn run build
```

### Run your tests
```
yarn run test
```

### Lints and fixes files
```
yarn run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


https://dev.to/hasurahq/vue-and-graphql-with-hasura-video-course-3mpp

https://docs.hasura.io/1.0/graphql/manual/getting-started/heroku-simple.html


frontend (vue)
http(s)://vue-hasura-cms-mtc.codeanyapp.com

backend (hasura)
https://vue-hasura-cms.herokuapp.com/console

optional 
https://elements.heroku.com/addons/newrelic


postgres enum examples:
https://docs.hasura.io/1.0/graphql/manual/schema/enums.html
CREATE TYPE film_status AS ENUM ('future', 'present', 'past');

ALTER TABLE film
  ALTER COLUMN status TYPE film_status using status::film_status;

ALTER TABLE articles
    RENAME TO article