#Toy App to Learn **User Authentication** with the `Devise` Gem

##The goals for this app are to:
* Learn `Devise` for `Rails 4`
* Create a user authentication framework
* Only allow a user to signup once they confirm via a confirmation email
* Send a confirmation email from both _dev_ and _prod_ enviroments

###Install `Devise` Gem and Setup Authentication Framework
* Followed instructions on: [The Devise GitHub page](https://github.com/plataformatec/devise)
* Wacthed tutorials [here](https://www.youtube.com/watch?v=qY5HccvIuS4) and [here](https://www.youtube.com/watch?v=3zvyeEYXT78)

###Some Devise Configuration
* Followed tutorial [here](https://www.youtube.com/watch?v=YnGuALpJN1M)
* Go to migration file and uncomment the `confirmable` fields
* If you messed up, like I did, run `rake db:rollback`, then uncomment the fields and run `rake db:migrate` again
* Add `:confirmable` to `models/users.rb`
* Set configuration in `environments/development.rb` and `environments/production.rb`
* Add `ActionMailer` configuration to new file `initializers/setup_mail.rb`

###Install _SendGrid_ Heroku Add-on
* `heroku addons:create sendgrid:starter`
* Added `gem "figaro"` and followed instructions on: [The Figaro GitHub page](https://github.com/laserlemon/figaro)
* Setup up `Enviroment Variables` for SendGrid username and password

###Deploy to Heroku
* Deployed app to Heroku
* Remember to run `heroku run rake db:migrate`

**It works!!**
