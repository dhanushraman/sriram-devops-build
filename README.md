const app = require('express')();
app.get('/',(req ,res) =>
res.json([message: 'message: 'docker is easy' ])
);
FROM NODE
WORKDIR/app
COPY packages.json./
copy . .
ENV PORT=8080
EXPOSE 8080
CMD ("npm" , "start")
