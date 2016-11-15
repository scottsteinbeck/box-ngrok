# box-ngrok

### Ngrok integration with CommandBox

## Usage
Use the commands that come with this module to start and stop Ngrok shares.
### Start a share
```bash
server share start
# or
share
```

It will:

1. Start the CommandBox server if it is not already running.
2. Start Ngrok using the embedded binaries for your platform.
3. Stop any currently open Ngrok tunnels (since the free version only allows one at a time).
4. Create the new Ngrok tunnel.
5. Display the share url.
6. Open the share url in the browser.

### Stop a share
```bash
server share stop
```

If you stop a server that is being shared, the Ngrok tunnel will be closed for you.


Great for testing integration with 3rd party systems (like Stripe webhooks) while still developing on localhost!
