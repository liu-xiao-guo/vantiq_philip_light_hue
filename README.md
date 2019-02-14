This is philip light control application in Nodejs on Vantiq platform.

1) A REST API server running at port 9000
2) MQTT protocol is used for monitoring the light

In order to get it running, you need to change the following place in the app.js file

const settings = {
    port: 1883,
    keepalive: 1000,
    protocolId: 'MQIsdp', // already tried 'MQTT' with protocol version 4
    protocolVersion: 3,
    clientId: 'a random id',
    username: 'YOUR USERNAME',
    password: 'YOUR PASSWORD'
}
