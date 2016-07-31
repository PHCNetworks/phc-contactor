[![security](https://hakiri.io/github/PHCNetworks/phc-contactor/master.svg)](https://hakiri.io/github/PHCNetworks/phc-contactor/master)
[![Code Climate](https://codeclimate.com/github/PHCNetworks/phc-contactor/badges/gpa.svg)](https://codeclimate.com/github/PHCNetworks/phc-contactor)
[![Issue Count](https://codeclimate.com/github/PHCNetworks/phc-contactor/badges/issue_count.svg)](https://codeclimate.com/github/PHCNetworks/phc-contactor)
[![Gem Version](https://badge.fury.io/rb/phccontactor.svg)](https://badge.fury.io/rb/phccontactor)

### PHCContactor(2) (Rails Contact Us Mailer Form) Documentation
PHCContactor(2) is a pre-configured contact form using ActionMailer.
  
- Customizable form using standard Bootstrap or HTML code.  
- Compatible with any mailer service using ActionMailer.  
  
#### Step 1 - Add PHCContactor Engine to your gemfile  
  
	gem 'phccontactor', '~> 2.0', '>= 2.0.3'
	bundle install
  
#### Step 2 - Configure ActionMailer 
  
* Configure ActionMailer in your Production.rb with any service.  
  
#### Step 3 - Recompile Assets  
PHCContactor included Views & UI requires Bootstrap and FontAwesome.
  
	rails assets:clobber
	rails assets:precompile

#### Step 4 - Generate Contact Form View (Customization)  
  
	rails generate phccontactor:views
  
#### Step 5 - Setup ENV Variables  
  
	ENV["PHC_CONTACTOR_SENDER"]  
  
