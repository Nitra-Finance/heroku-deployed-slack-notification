# Heroku deployed slack notification
A Heroku buildpack for sending salck notification


## To use the deploy notification
* Use Heroku CLI to enable `<app-name>` runtime dyno metadata ->  `heroku labs:enable runtime-dyno-metadata -a <app-name> & heroku labs:enable runtime-dyno-build-metadata -a <app-name>`
* Set Config Vars -> key: `SLACK_WEBHOOK_URL` , value: A Slack Webhook url you created
* Add buildpack -> [Heroku deployed slack notification](https://github.com/Nitra-Finance/heroku-deployed-slack-notification.git)
* Then check that the buildpack order must be the last one.
