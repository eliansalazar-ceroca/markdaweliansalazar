## Documetación del bot de Discord

![logotipo de discord](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSUg8q_pE8Mb8_eGNLru-dJcUeXpmD78883rzCOUAKwfQ&s=10)

puedes registrar tu aplicacion al [portal de desarolladores de discord](https://discord.com/developers/applications)

para hacer que el bot responda, escuchamos el evento `messageCreate` y utilizamos el metodo `message.reply()`.

```JAVASCRIPT
client.on('messageCreate', message => {
if (message.content === 'ping') {
message.reply('pong!');
}
});
```