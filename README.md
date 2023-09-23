# alphabot-api-example

A basic nodejs + express example of receiving and valdiating webhooks with the [Alphabot API](https://api.alphabot.app) for real-time data updates from [Alphabot.app](https://www.alphabot.app)

Steps to run & receive webhook events locally after cloning or forking this repo: 

1. Copy `.env.local.example` and paste, leaving the file name as just `.env.local`
2. Populate the `ALPHABOT_API_KEY` in the new file with your value from your [Alphabot profile](https://alphabot.app/#profile-developer)
3. Run `yarn && yarn start` - this will start the node server at port 8080
4. Run `ngrok http 8080` in another terminal, after setting up a free [ngrok](https://ngrok.com/) account (or your choice of localhost tunneling services) to make your webhook a public URL on the internet.
5. Copy the Forwarding url (should end with .ngrok-free.app) and paste it into your Webhook url in your [Alphabot profile](https://alphabot.app/#profile-developer)
6. You are now receiving Alphabot webhooks and receiving real time data updates. Congratulations!

You could easily connect your fork to a new website at [render.com](https://render.com) or similar if you prefer to run the node server in the cloud.
