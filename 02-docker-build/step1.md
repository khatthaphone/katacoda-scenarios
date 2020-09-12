# ຂຽນ Code

ສ້າງໄຟລ໌ index.js

```
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

ສ້າງ start script ໃນ package.json

```
...
"scripts": {
    "start": "node index.js",
    ...
}
...
```

ລອງ start
`npm run start`