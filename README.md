# NestJS + Socket.IO demo

Demo de backend realtime con **NestJS** y **Socket.IO**: gateway WebSocket, rooms y un adaptador de sockets autenticados.

**Live:** [test-nestjs-socketio.vercel.app](https://test-nestjs-socketio.vercel.app)

## Qué muestra

- API HTTP NestJS (`@nestjs/platform-express`)
- Gateway WebSocket con `@nestjs/websockets` + `@nestjs/platform-socket.io`
- Rooms y eventos tipados bajo `src/sockets/`
- Adaptador de autenticación para sockets (`authenticated-socket.adapter.ts`)
- Helmet habilitado en el bootstrap

Es un proyecto de práctica/demo (no un producto en producción), útil para ver un patrón Nest + realtime.

## Stack

- TypeScript
- NestJS 9
- Socket.IO
- Helmet

## Correr local

```bash
npm install
npm run start:dev
```

Build / prod:

```bash
npm run build
npm run start:prod
```

## Estructura relevante

```
src/
  main.ts
  app.module.ts
  sockets/
    sockets.gateway.ts
    rooms.ts
    events.ts
    authenticated-socket.adapter.ts
```

## Autor

[Andrés Navarro](https://github.com/Rompni) · [andresnavarro.dev](https://www.andresnavarro.dev)
