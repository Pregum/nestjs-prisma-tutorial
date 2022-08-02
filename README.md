
## Description

.https://docs.nestjs.com/recipes/prisma#issues-with-enableshutdownhooks

上記ページを参考にNestJSとPrismaを使用したサンプルリポジトリです。

ルーティングは下記の通りです。

```
* GET
  /post/:id: Fetch a single post by its id
  /feed: Fetch all published posts
  /filter-posts/:searchString: Filter posts by title or content
* POST
  /post: Create a new post
    Body:
      title: String (required): The title of the post
      content: String (optional): The content of the post
      authorEmail: String (required): The email of the user that creates the post
/user: Create a new user
  Body:
    email: String (required): The email address of the user
    name: String (optional): The name of the user
*PUT
  /publish/:id: Publish a post by its id
* DELETE
  /post/:id: Delete a post by its id

```


## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## .envの設定

.envファイルをルートディレクトリに追加し、.envファイル内に下記1行を追加してください

```.env
DATABASE_URL="file:./dev.db"
```


## License

[MIT licensed](LICENSE).
