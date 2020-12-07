# ຂຽນ Code

ສ້າງໄຟລ໌ index.js

## ກ່ອນອືນໝົດ ໃຫ້ສ້າງໂປຣເຈັກ NodeJS ຂຶ້ນມາກ່ອນ

`top`{{
    mkdir nodeapp
    cd nodeapp
    npm init
    npm install --save express
}}

ສ້າງໄຟລ໌ app.js

```js
const express = require('express');
const app = express();
    app.get('/', (req, res) => {
    return res.send('<html><body>Sample made with ♥️</body></html>');
});
const port = process.env.port | 8080;
app.listen(port, () => {
    console.log('listing on port:', port);
});
```

ເພີ່ມ start script ໃນ package.json

```js
...
"scripts": {
    "start": "node index.js",
    ...
}
...
```

ລອງ start
`npm run start`
