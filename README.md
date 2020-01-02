This is a summary from development to production based on my 7+ years working experience using Ruby on Rails

If you have any suggestion, please create a issue or pullrequest to help me to improve this summary

# Development
Use Ruby on Rails as main web framework
### Version Control Flow
- Checkout a new local branch for a JIRA/Other issue: feature/JIRA-1-add-product
- Push local branch to Github and create a pullrequest
- Pass integration test then deploy to staging and do manual test
- Invite code review
- Merge to master then deploy to staging and test manually again
- Finally deploy to production

Note: 
- Rebase to master branch when needed
- Use [Lefthook](https://evilmartians.com/chronicles/lefthook-knock-your-teams-code-back-into-shape) to unify git hooks for a project

### Test
- [RSpec](https://github.com/rspec/rspec-rails) for unit and integration test
- [Rails testing](https://guides.rubyonrails.org/testing.html)
###

### Continuous Integration
- [CircleCI](https://circleci.com/)

### Rails
- Use [Rubocop](https://github.com/airbnb/ruby/tree/master/rubocop-airbnb) to unify the common rule accrossing a project
- Get updates from [GoRails](https://gorails.com)
- Use less gems as possible. Check [recommended gems](https://gorails.com/tool_categories)
- Be consistent with a [Ruby style](https://github.com/airbnb/ruby)

### Editor and other tools
- [VIM from thoughtbot](https://thoughtbot.com/upcase/vim)
- [Microsoft Visual Studio Code](https://code.visualstudio.com/)

### Communication
- Slack
- Email: [SendGrid](https://sendgrid.com/)
- Push Notification: [OneSignal](https://onesignal.com/)

# Production
### Deployment
- [Heroku](https://www.heroku.com/) for easy to deploy but more expensive
- EngineYard
- VPS like Linode, Digital Ocean

### Monitoring
- Error Tracking: [HoneyBadger](https://www.honeybadger.io/)
- Performance Monitoring: [NewRelic](https://newrelic.com/)
- Logging: [AWS CloudWatch](https://aws.amazon.com/cloudwatch/)

### Others
- [Production checklist](https://github.com/ankane/production_rails)



# References:
- https://thoughtbot.com/playbook
- My 3-year working experience at [Lixibox](https://www.lixibox.com)
