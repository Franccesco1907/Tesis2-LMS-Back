# Tesis2-LMS-Back

API Express/Mongoose para alumnos, docentes y administración. Basada en [LMS-Backend-API](https://github.com/omob/LMS-Backend-API); cliente: [Tesis2-LMS-Front](https://github.com/Franccesco1907/Tesis2-LMS-Front).

1. Ejecutar `npm ci`.
2. Configurar MongoDB y un secreto propio en `app/config/development.json` (JSON sin comentarios):

```json
{"host":"http://localhost:3000","dbURI":"mongodb://127.0.0.1:27017/lms","sessionSecret":"REEMPLAZAR_CON_SECRETO_LOCAL","tokenExpire":5300,"port":3000,"domain":"example.edu"}
```

3. Ejecutar `node server.js`. Rutas en `/api`, `/api/admin`, `/api/student`, `/api/staff` y `/api/lecturer`.

Con `NODE_ENV=production`, el código lee `host`, `dbURI`, `sessionSecret`, `PORT` y `tokenExpire` del entorno; el dominio se define en `app/config/index.js`. No publicar secretos ni reutilizar los valores versionados.

Datos de desarrollo heredados: [colecciones](https://1drv.ms/u/s!AtuFwKw_48h8qUm0OLgfTB264g2p?e=dx2X2w). Su disponibilidad y compatibilidad no están verificadas.
`npm test` es un marcador que termina con error; no hay suite automatizada. Licencia: [MIT](LICENSE).
