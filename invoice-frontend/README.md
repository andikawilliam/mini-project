# Invoice Frontend

## How to use it

Requires:
Node JS (>= 12.x)

**Step 1** - Clone the project

```bash
$ git clone "this repo"
$ cd invoice-frontend
```

<br >

**Step 2** - Install dependencies via NPM or yarn

```bash
$ npm i
```

<br />

**Step 3** - Start in development mode

```bash
$ npm run start 
```

## Configure the backend server

**API Server URL** - `src/config/constant.js` 

```javascript
const config = {
    ...
    API_SERVER: 'http://localhost:5000/api/'  // <-- The magic line
};
```

<br />

**API Server Descriptor** - POSTMAN Collection

The API Server signature is provided by the [Unified API Definition](https://docs.gmail.com/boilerplate-code/api-unified-definition)

- [API POSTMAN Collection](https://github.com/app-generator/api-server-unified/blob/main/api.postman_collection.json) - can be used to mock (simulate) the backend server or code a new one in your preferred framework. 

<br />

### Compile the API Server

**Step 1** - Clone the project

```bash
$ git clone https://github.com/app-generator/api-server-nodejs.git
$ cd api-server-nodejs
```

**Step #2** - Install dependencies via NPM or Yarn

```bash
$ npm i
```

**Step 3** - Run the SQLite migration via TypeORM

```
$ npm run typeorm migration:run
```

**Step 4** - Start the API server (development mode)

```bash
$ npm run dev
```

The API server will start using the `PORT` specified in `.env` file (default 5000).

<br /> 

---
