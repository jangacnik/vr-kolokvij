# Kolokvij naloga - Node-RED
# Getting started with Node-RED and Docker
Install docker desktop and run command:
```
docker run -it -p 1880:1880 -v node_red_data:/data --name mynodered nodered/node-red
```
This will create a runnign docker image on [localhost](http://localhost:1880).

To start the docker image use:
```docker start mynodered```

To stop node-RED use
```docker stop mynodered```

For more info visit: [Node-RED docs](https://nodered.org/docs/getting-started/docker#using-named-data-volumes)

# Example Flow

Install the discord nodes with the command:

```npm install node-red-contrib-discord-advanced```

Download the [flows.json](https://github.com/jangacnik/vr-kolokvij/blob/main/flows.json). 

Go to your Node-RED flow editor and click on the burger menu on the top right

![image](https://github.com/jangacnik/vr-kolokvij/assets/40426150/8437197a-73c5-4175-96a4-4752a6e28aad)

Choose import and select the downloaded flows.json file. The imported flow should look like this.
![image](https://github.com/jangacnik/vr-kolokvij/assets/40426150/32534cfb-f92a-4d46-b5b4-ad7de4af0d1d)

Select a discord node in the flow and choose "Add new discord token" in the dropdown and click on the edit icon:
![image](https://github.com/jangacnik/vr-kolokvij/assets/40426150/25ce9669-7b9b-48b7-be40-d117235c70b3)

Add the token into the field and choose a name for the discord bot.

![image](https://github.com/jangacnik/vr-kolokvij/assets/40426150/52fdb027-6a2d-49e1-be3c-c18199d76c05)

You can find your token in your [discord developer portal page](https://discord.com/developers/applications) => My Appliactions => [My app] => Bot => Token
Note that all Privileged Gateway Intents must be enabled
