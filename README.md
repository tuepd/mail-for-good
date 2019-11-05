# Mail for Good

[![Join the chat at https://gitter.im/FreeCodeCamp/mail-for-good](https://badges.gitter.im/FreeCodeCamp/mail-for-good.svg)](https://gitter.im/FreeCodeCamp/mail-for-good?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

*Please be aware that Mail for Good is currently in beta.*

Looking to contribute? Read our [developer setup guide](https://github.com/freeCodeCamp/Mail-for-Good/wiki/Setup-for-development).

---

![Image showing Mail 4 Good](docs/resources/hero.png)

An app for sending millions of emails as cheaply as possible. Mail for Good uses AWS Simple Email Service to send bulk emails at $0.10 per 1000 emails.

Mail for Good is fast and memory efficient, currently sending over 100 emails per second on a 1gb Digital Ocean VPS.

We've used Mail for Good to deliver newsletters to hundreds of thousands of campers per week.

## Sounds good? Give it a try!
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/freeCodeCamp/mail-for-good/tree/heroku/stable)

"My instance is deployed, what now?"

In [setting_up.md](./docs/setting_up.md) you'll find how to connect, create your admin account and set up your AWS credentials allowing you to send your first blast.


## What does Mail for Good do?

With Mail for Good you can:

- Send email campaigns of unlimited size.
- Import emails saved in CSV format.
- Create templates to reuse for convenience when sending email campaigns.
- Track bounce rate and other standard metrics. You can also insert tracking pixels and unsubscribe links at the click of a button.
- Add custom fields to imported email lists such as names or cities.
- Grant other users (limited or otherwise) permissions to use your account on your behalf.
- Add embedded HTML newsletter sign up forms to your site. These are snippets of code that will let your users sign up with you at the click of a button.

### Performance

We're currently sending weekly email blasts of over 800,000 emails in 4 hours on a $10 per month Digital Ocean VPS with 1gb memory and 1 core processor.

Mail for Good is fast and scales to the rate limit enforced by AWS.

### Why are we doing this?

We want to help nonprofits manage their email campaigns as inexpensively as possible, and have full control over their data.

### How to install locally
[**local deployment guide.md**](./docs/local_deploy.md).

# Setting up

## Creating your account and deleting the default admin account

To connect for the first time you'll have to use the default admin account. The email is "admin@admin.com" and the password is "admin".

In the menu on the left of your screen you'll see the "accounts management section". There you'll find a form to create your first admin account and another to delete the default one.

## Retrieving your AWS credentials

Here is a video from Quincy showing how to get your Amazon credentials to allow your instance to send through the Amazon Simple Email Service.
https://www.youtube.com/watch?v=_7U03GVD4a8

## Last step: Getting out of Amazon's sandbox mode

Right now you can only send emails to the verified address you provided during the last step.

Here is a link on how to proceed.
https://docs.aws.amazon.com/ses/latest/DeveloperGuide/request-production-access.html

When filling the form, be aware that they will want to know about how you plan to handle bounces and complaints. You will send your emails through their service and if you let the complaints pile up you will lower the reputation of their servers, degrading their service. Show them you understand that. Be serious and honest while filling your submission.



### Troubleshooting

We're keen to tackle any issues people encounter. If you experience any problems, please create an issue and we'll get back to you.

### How to contribute

Found a bug? Please let us know by [creating an issue](https://github.com/freeCodeCamp/Mail-for-Good/issues/new).

We warmly welcome contributions from anyone. Check out our [how to contribute](https://github.com/FreeCodeCamp/nonprofit-email-service/blob/master/CONTRIBUTING.md) section to find out how you can do so.

### License

Copyright (c) 2018, freeCodeCamp.

This computer software is licensed under the [BSD-3-Clause](https://github.com/freeCodeCamp/Mail-for-Good/blob/master/LICENSE.md).
