#Toy App to Learn **User Authentication** with the `Devise` Gem

##Install `Devise` Gem and Setup Authentication Framework
* Followed instructions on: [The Devise GitHub page](https://github.com/plataformatec/devise)
* Wacthed tutorials: [here](https://www.youtube.com/watch?v=qY5HccvIuS4) and [here](https://www.youtube.com/watch?v=3zvyeEYXT78)

##Deploy to Heroku
* Deployed app to Heroku
* Remember to run `rake db:migrate`

###It works so far!

##Install _SendGrid_ Heroku Add-on
* `heroku addons:create sendgrid:starter`
* Setup `production.rb` per the [docs](https://devcenter.heroku.com/articles/sendgrid#ruby-rails)
* Setup `development.rb` per [this blog post](https://howilearnedrails.wordpress.com/2014/02/25/setting-up-email-in-a-rails-4-app-with-action-mailer-in-development-and-sendgrid-in-production-using-heroku/comment-page-1/) since I want to send emails in development
