# RSVP App

This is an application I built for a friend's wedding to collect guest's RSVPs and contact details. It is built using [Ruby on Rails] with SMS and email functionality provided by [Twilio] and [SendGrid]. The admin dashboards were created using the [Administrate] Gem.

[Ruby on Rails]: https://rubyonrails.org/
[Twilio]: https://www.twilio.com/
[SendGrid]: https://sendgrid.com/
[Administrate]: https://github.com/thoughtbot/administrate

## Features

- Simple guest registration with confirmation via SMS
- Guests may update their details at any time with login codes sent via SMS
- Manage guests with the included administration dashboard
- Send email notifications to guests

## System dependencies

- Ruby 2.4.0+
- PostgreSQL 10+
- [Bundler](https://bundler.io/)

## Local project setup and configuration

```sh
# Clone this Git repo
git clone https://github.com/i-like-robots/rsvp-app.git && cd rsvp-app

# Add local environment configuration
cp .env.example .env && open .env

# Install application dependencies
bundle install --without=production

# Setup database (ensure PostgreSQL service is running)
bundle exec rake db:setup

# Run the development server
bundle exec rails s
```

## Screenshots

<img alt="" src="https://user-images.githubusercontent.com/271645/41441093-17c4dd54-7029-11e8-8dab-de4107626191.png">
<img alt="" src="https://user-images.githubusercontent.com/271645/41441094-17e2927c-7029-11e8-9191-9fd36dbeadf9.png">
<img alt="" src="https://user-images.githubusercontent.com/271645/41441095-17fbf35c-7029-11e8-9d14-64488f400865.png">
