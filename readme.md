## facematch-styling

Use this app to configure and test FaceMatch UI customizations. Once you have the UI looking the way you want, provide the `config.json` file to Verisoul. 

### Install
```bash
npm install
```

### Run
```bash
npm start
```

### Generate session_id
Use your api key to manually generate a session_id in the sandbox environment using the `/liveness/session` endpoint. 


### Load Website
Open `http://localhost:3000?custom_config=true&session_id=<session_id>` in your browser.

### Update Config
Update `config.json` in the `public` folder and reload the site to see the new UI


### Troubleshooting
If you reload the website with anything in the path (/Face or /Error) the local server won't be able to resolve the path.
When refreshing the page, make sure to only refresh `http://localhost:3000?custom_config=true&session_id=<session_id>`