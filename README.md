### PHCContactor(1) (Rails Contact Us Mailer Form) Documentation
PHCContactor is a pre-configured contact form using ActionMailer.
  
* Customizable form using standard Bootstrap or HTML code.  
* Compatable with any mailer service using ActionMailer.  
  
#### Step 1 - Add PHCContactor Engine to your gemfile  
  
	gem 'phccontactor', '~> 1.0', '>= 1.0.7' 
	bundle install
  
#### Step 2 - Configure ActionMailer 
  
* Configure ActionMailer in your Production.rb with any service.  
  
#### Step 3 - Recompile Assets  
PHCContactor included Views & UI requires Bootstrap and FontAwesome.
  
	rake assets:clobber
	rake assets:precompile

#### Step 4 - Generate Contact Form View (Customization)  
  
	rails generate phccontactor:views
  
#### Step 5 - Setup ENV Variables  
  
	ENV["PHC_CONTACTOR_SENDER"]  
  