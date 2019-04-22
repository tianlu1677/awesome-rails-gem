# Awesome Rails Gem [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
收集自己使用过的并且出色的gem

* [Rails Gem List](#rails-gem-list)
  * [User](#user)
    - [Devise](https://github.com/plataformatec/devise/) 用户登录注册
    - [Clearance](https://github.com/thoughtbot/clearance) 简易版本的用户的登录注册
    - [Devise JWT](https://github.com/waiting-for-dev/devise-jwt) 用户登录注册使用token
    - [Pundit](https://github.com/elabs/pundit) 权限验证， 推荐使用这个
    - [cancancan](https://github.com/CanCanCommunity/cancancan) cancancan
  * [Active Record](#active-record)
    - [Enumerize](https://github.com/brainspec/enumerize) 列出所有可能的列
    - [FriendlyId](https://github.com/norman/friendly_id) url友好
    - [paranoia](https://github.com/rubysherpas/paranoia) 软删除
  * [Server](#server)
    - [puma]
    - [nginx]
    - [Docker]
  * [Cache](#cache)
    - [redis]() redis数据库
    - [redis-objects]() redis的对象，方便存储临时性数据
    - [redis-rails]() 使用redis做rails的缓存
    - [second_level_cache]() 二级缓存
    - [actionpack-action_caching]()  action级别的缓存
  * [Database](#database)
    - [pg]() postgres 数据库
    - [pghero]() 数据库监控
    - [rails_db](https://github.com/igorkasyanchuk/rails_db) 在线直接查询数据库
    - [mysql2]() mysql数据库

  * [Plugins](#plugins)
    - [ActsAsTaggableOn](https://github.com/mbleigh/acts-as-taggable-on) 打标签
    - [kaminari](https://github.com/amatsuda/kaminari) 分页
  * [API](#api)
    - [ActiveModel::Serializers](https://github.com/rails-api/active_model_serializers)
    - [Jbuilder](https://github.com/rails/jbuilder)
    - [Jbuilder_cache_multi]()
    - [rest-client](https://github.com/rest-client/rest-client)
    - [rack-attack]() 防止被攻击
    - [rack-cors]() 跨域
    - [api-pagination] api分页

  * [Email](#email)
  * [File Uploading](#file-uploading)
    - [Carrierwave](https://github.com/carrierwaveuploader/carrierwave) 文件上传
    - [Carrierwave qiniu] 文件上传到七牛
    - [Carrierwave aliyun] 文件上传到阿里云
    - [carrierwave_backgrounder](https://github.com/lardawge/carrierwave_backgrounder) 
    - [MiniMagick](https://github.com/minimagick/minimagick) 裁剪图片
  * [Searching](#searching)
    - [ransack](https://github.com/activerecord-hackery/ransack) 对象级别的搜索
    - [pg_search](https://github.com/Casecommons/pg_search) 全局搜索
    
  * [Scheduled/Recurrence Jobs](#scheduledrecurrence-jobs)
    - [sidekiq](https://github.com/tobiassvn/sidetiq) 后台任务队列
    - [sidekiq-cron](https://github.com/ondrejbartas/sidekiq-cron) 定时任务队列    
    - [sidekiq-failures](https://github.com/mhfs/sidekiq-failures)  队列出错的详细信息
    - [Whenever](https://github.com/javan/whenever) - 可不用sidekiq，crontab
  * [View Helper](#view-helper)
    - [Simple Form](https://github.com/plataformatec/simple_form) 
    - [cocoon](https://github.com/nathanvda/cocoon)  嵌套form的表单
  * [Environment Variables](#environment-variables)
    - [Figaro](https://github.com/laserlemon/figaro) 使用环境变量来存储
  * [Admin Panel](#admin-panel)
    - [administrate](https://github.com/thoughtbot/administrate) 简易后台程序
  * [Logging](#logging)
  * [Debug](#debug)
    - [pry]
    - [pry-rails]

  * [Coding Style](#coding-style)
    - [RuboCop](https://github.com/bbatsov/rubocop)
  * [Testing](#testing)
    - [rspec-rails](https://github.com/rspec/rspec-rails) 
    - [factory_bot_rails](https://github.com/thoughtbot/factory_bot_rails) 创建测试对象
    - [Database Cleaner](https://github.com/DatabaseCleaner/database_cleaner) 清除数据库
    - [shoulda-matchers](https://github.com/thoughtbot/shoulda-matchers)
    - [Timecop](https://github.com/travisjeffery/timecop) 锁定时间
    - [brakeman](https://github.com/presidentbeef/brakeman) 检查语法安全
    - [bundle-audit](https://github.com/rubysec/bundler-audit) 检查gem是不是有安全性的版本更新
  * [Production](#production)
  * [Error Logging](#error-logging)
  * [Frontend](#frontend)
    - [slim]
    - [jquery-rails]
    - [bootstrap] 样式效果
    - [bootstrap-datepicker-rails] 选择日期
    - [select2-rails] 选择
    - [coreui] 后台的样式效果
    - [toastr-rails] 消息提醒
    - [jsoneditor-rails] json编辑器
    - [richexitor] 富文本编辑器

## User

### Authentication
* [Devise](https://github.com/plataformatec/devise/) - Devise is a flexible authentication solution for Rails based on Warden.
* [Clearance](https://github.com/thoughtbot/clearance) - Rails authentication with email & password.
* [Devise JWT](https://github.com/waiting-for-dev/devise-jwt) - JWT FOR Devise


### Authorization
* [Pundit](https://github.com/elabs/pundit) - Pundit provides a set of helpers which guide you in leveraging regular Ruby classes and object oriented design patterns to build a simple, robust and scaleable authorization system.
* [cancancan](https://github.com/CanCanCommunity/cancancan) - Continuation of CanCan, the authorization Gem for Ruby on Rails.CanCan is an authorization library for Ruby on Rails which restricts what resources a given user is allowed to access. All permissions are defined in a single location (the Ability class) and not duplicated across controllers, views, and database queries.


### Omniauth
* [omniauth-facebook](https://github.com/mkdynamic/omniauth-facebook)
* [omniauth-google-oauth2](https://github.com/zquestz/omniauth-google-oauth2)
* [omniauth-weibo-oauth2](https://github.com/beenhero/omniauth-weibo-oauth2)
* [omniauth-twitter](https://github.com/arunagw/omniauth-twitter)
* [omniauth-github](https://github.com/intridea/omniauth-github)
* [omniauth-linkedin-oauth2](https://github.com/decioferreira/omniauth-linkedin-oauth2)

## Database
* [pg]()
* [pghero]
* [rails_db](https://github.com/igorkasyanchuk/rails_db) - Rails Database Viewer and SQL Query Runner

## Cache
* [redis]
* [redis-objects]
* [redis-rails]
* [second_level_cache]
* [actionpack-action_caching]

## API about


## Active Record
* [Enumerize](https://github.com/brainspec/enumerize) - Enumerated attributes with I18n and ActiveRecord/Mongoid support. It can be integrated with Simple Form.
* [counter_culture](https://github.com/magnusvk/counter_culture) - Turbo-charged counter caches for your Rails app. Huge improvements over the Rails standard counter caches.
* [custom_counter_cache](https://github.com/cedric/custom_counter_cache) - A simple approach to creating a custom counter cache that can be used across multiple models.

* [FriendlyId](https://github.com/norman/friendly_id) - FriendlyId is the “Swiss Army bulldozer” of slugging and permalink plugins for ActiveRecord. It allows you to create pretty URL’s and work with human-friendly strings as if they were numeric ids for ActiveRecord models.
* [AASM](https://github.com/aasm/aasm) - State machines for Ruby classes (plain Ruby, Rails Active Record, Mongoid).
* [PaperTrail](https://github.com/airblade/paper_trail) - PaperTrail lets you track changes to your models' data. It's good for auditing or versioning.
* [paranoia](https://github.com/rubysherpas/paranoia) - ActiveRecord plugin allowing you to hide and restore records without actually deleting them.
* [Validates](https://github.com/kaize/validates) - Validates provides collection of useful custom validators for Rails applications, including:
  * EmailValidator
  * UrlValidator
  * SlugValidator
  * MoneyValidator
  * IpValidator
  * AssociationLengthValidator
  * AbsolutePathValidator
  * UriComponentValidator
  * ColorValidator
  * EanValidator (EAN-8 & EAN-13)
* [globalize](https://github.com/globalize/globalize) - Rails I18n de-facto standard library for ActiveRecord model/data translation.
* [deep_cloneable](https://github.com/moiristo/deep_cloneable) - This gem gives every ActiveRecord::Base object the possibility to do a deep clone that includes user specified associations.
* [social_shares](https://github.com/Timrael/social_shares) - Check how many times url was shared in social networks.
* [public_activity](https://github.com/chaps-io/public_activity) - Easy activity tracking for models - similar to Github's Public Activity.
* [goldiloader](https://github.com/salsify/goldiloader) - Automatic ActiveRecord eager loading to reduce the number of database queries run by your application.
* Tagging
  * [ActsAsTaggableOn](https://github.com/mbleigh/acts-as-taggable-on) - A tagging plugin for Rails applications that allows for custom tagging along dynamic contexts.
  * [closure_tree](https://github.com/mceachen/closure_tree) - Easily and efficiently make your ActiveRecord models support hierarchies.
* [ActionStore](https://github.com/rails-engine/action-store) - Store different kind of actions (Like, Follow, Star, Block ...) in one table via ActiveRecord Polymorphic Association.

## Plugins
* [Spreadsheet](https://github.com/zdavatz/spreadsheet) - Library is designed to read and write Spreadsheet Documents.
* [Chartkick](https://github.com/ankane/chartkick) - Chartkick helps your to create beautiful Javascript charts with one line of Ruby.
* [kaminari](https://github.com/amatsuda/kaminari) - A Scope & Engine based, clean, powerful, customizable and sophisticated paginator for Rails 3 and 4.
* [CKEditor](https://github.com/galetahub/ckeditor) - CKEditor is a WYSIWYG text editor designed to simplify web content creation. It brings common word processing features directly to your web pages. Enhance your website experience with our community maintained editor. [ckeditor.com](http://ckeditor.com)
* [HTML::Pipeline](https://github.com/jch/html-pipeline) - GitHub HTML processing filters and utilities. This module includes a small framework for defining DOM based content filters and applying them to user provided content.
* [Slack Notifier](https://github.com/stevenosloan/slack-notifier) is a simple wrapper to send notifications to [Slack](https://slack.com/) webhooks.
* [Rails ERD](https://github.com/voormedia/rails-erd) - Generate Entity-Relationship Diagrams for Rails applications.
* [Parity](https://github.com/thoughtbot/parity) - Shell commands for development, staging, and production parity for Heroku apps.
* [Airbrussh](https://github.com/mattbrictson/airbrussh) - Airbrussh pretties up your SSHKit and Capistrano output

## API
* [ActiveModel::Serializers](https://github.com/rails-api/active_model_serializers) - Serializer brings convention over configuration to your JSON generation.
* [Jbuilder](https://github.com/rails/jbuilder)
* [jbuilder_cache_multi]()
* [rest-client](https://github.com/rest-client/rest-client)
* [api-pagination]
* [rack-attack]()
* [rack-cors]()

## Email
* [letter_opener](https://github.com/ryanb/letter_opener) - Preview mail in the browser instead of sending.

## File Uploading
* [Carrierwave](https://github.com/carrierwaveuploader/carrierwave) - Carrierwave is a classier solution for file uploads for Rails, Sinatra and other Ruby web frameworks.
  * [carrierwave_backgrounder](https://github.com/lardawge/carrierwave_backgrounder) - Offload CarrierWave's image processing and storage to a background process using Delayed Job, Resque, Sidekiq, Qu, Queue Classic or Girl Friday.
* [MiniMagick](https://github.com/minimagick/minimagick) - MiniMagick is a ruby wrapper for ImageMagick or GraphicsMagick command line.


## Searching
* [ransack](https://github.com/activerecord-hackery/ransack) - Ransack enables the creation of both simple and advanced search forms for your Ruby on Rails application.
* [elasticsearch-rails](https://github.com/elastic/elasticsearch-rails) - Elasticsearch integrations for ActiveModel/Record and Ruby on Rails.

* [pg_search](https://github.com/Casecommons/pg_search) - pg_search builds ActiveRecord named scopes that take advantage of PostgreSQL's full text search
* [searchkick](https://github.com/ankane/searchkick) - Intelligent search made easy with Rails and Elasticsearch.

## Scheduled/Recurrence Jobs
* [Whenever](https://github.com/javan/whenever) - Whenever is a Ruby gem that provides a clear syntax for writing and deploying cron jobs.
* [Sidekiq](https://github.com/mperham/sidekiq) - Simple, efficient background processing for Ruby.
  * [sidetiq](https://github.com/tobiassvn/sidetiq) - Recurring jobs for sidekiq.
  * [sidekiq-cron](https://github.com/ondrejbartas/sidekiq-cron) - Scheduler / Cron for Sidekiq jobs
  * [sidekiq-scheduler](https://github.com/Moove-it/sidekiq-scheduler) - Lightweight job scheduler extension for Sidekiq
  * [sidekiq-failures](https://github.com/mhfs/sidekiq-failures) Sikekiq的错误展示
* [Sucker Punch](https://github.com/brandonhilkert/sucker_punch) - Sucker punch is a single-process Ruby asynchronous processing library. 简单的可以不用sidekiq而直接使用。

## View Helper
* [Simple Form](https://github.com/plataformatec/simple_form) - Simple form aims to be as flexible as possible while helping you with powerful components to create your forms. The basic goal of Simple Form is to not touch your way of defining the layout, letting you find the better design for your eyes.

* [meta-tags](https://github.com/kpumuk/meta-tags) - Search Engine Optimization (SEO) plugin for Ruby on Rails applications.

* [cocoon](https://github.com/nathanvda/cocoon) - Dynamic nested forms using jQuery made easy

## Environment Variables
* [Figaro](https://github.com/laserlemon/figaro) - Figaro is very simple, Heroku-friendly Rails app configuration using ENV and a single YAML file.

## Admin Panel
* [administrate](https://github.com/thoughtbot/administrate) - A Rails engine that helps you put together a super-flexible admin dashboard.

## Logging
* [Impressionist](https://github.com/charlotte-ruby/impressionist) - Impressionist can log page impressions (technically action impressions), but it is not limited to that. You can log impressions multiple times per request. And you can also attach it to a model. The goal of this project is to provide customizable stats that are immediately accessible in your application as opposed to using Google Analytics and pulling data using their API.
* [Ahoy](https://github.com/ankane/ahoy) - Ahoy provides a solid foundation to track visits and events in Ruby, JavaScript, and native apps.
* [Lograge](https://github.com/roidrage/lograge) - An attempt to tame Rails' default policy to log everything.

## Debug
* [byebug](https://github.com/deivid-rodriguez/byebug) - Byebug is a simple to use, feature rich debugger for Ruby 2. It uses the new TracePoint API for execution control and the new Debug Inspector API for call stack navigation, so it doesn't depend on internal core sources.
  * [pry-byebug](https://github.com/deivid-rodriguez/pry-byebug) - Pry navigation commands via byebug.
* [pry-rails](https://github.com/rweng/pry-rails) - Avoid repeating yourself, use pry-rails instead of copying the initializer to every rails project. This is a small gem which causes rails console to open pry. It therefore depends on pry.
* [awesome_print](https://github.com/awesome-print/awesome_print) - Awesome Print is a Ruby library that pretty prints Ruby objects in full color exposing their internal structure with proper indentation.
* [web-console](https://github.com/rails/web-console) - Web Console is a debugging tool for your Ruby on Rails applications.
* [spring](https://github.com/rails/spring) - Spring is a Rails application preloader. It speeds up development by keeping your application running in the background so you don't need to boot it every time you run a test, rake task or migration.

## Coding Style
* [RuboCop](https://github.com/bbatsov/rubocop) - Rubocop is a Ruby static code analyzer. Out of the box it will enforce many of the guidelines outlined in the community [Ruby Style Guide](https://github.com/bbatsov/ruby-style-guide).
* [Rails Best Practice](https://github.com/railsbp/rails_best_practices) - Rails best practice is a code metric tool to check the quality of rails codes.
* [Metric Fu]( https://github.com/metricfu/metric_fu) - A fist full of code metrics
* [Pronto](https://github.com/mmozuras/pronto) - Quick automated code review of your changes

## Testing
* [rspec-rails](https://github.com/rspec/rspec-rails) - Rspec-rails is a testing framework for Rails 3.x and 4.x.
* [Capybara](https://github.com/jnicklas/capybara) - Capybara helps you test web applications by simulating how a real user would interact with your app. And drivers:
  - [capybara-webkit](https://github.com/thoughtbot/capybara-webkit) - Capybara-webkit is a capybara driver that uses Webkit via QtWebkit.
  - [selenium-webdriver](https://github.com/vertis/selenium-webdriver) - Selenium-webdriver provides ruby bindings for WebDriver.
  - [poltergeist](https://github.com/teampoltergeist/poltergeist) - Poltergeist allows you to run your Capybara tests on a headless WebKit browser, provided by PhantomJS.
  - [page-object](https://github.com/cheezy/page-object) - Page-object is a simple gem that assists in creating flexible page objects for testing browser based applications.
* [factory_bot](https://github.com/thoughtbot/factory_bot) - Factory_bot is a fixtures replacement with a straightforward definition syntax, support for multiple build strategies (saved instances, unsaved instances, attribute hashes, and stubbed objects), and support for multiple factories for the same class (user, admin_user, and so on), including factory inheritance.
* [factory_bot_rails](https://github.com/thoughtbot/factory_bot_rails) - Factory_bot_rails provides Rails integration for factory_bot.
* [Database Cleaner](https://github.com/DatabaseCleaner/database_cleaner) - Database Cleaner is a set of strategies for cleaning your database in Ruby.Support ActiveRecord, DataMapper, Sequel, MongoMapper, Mongoid, CouchPotato, Ohm and Redis.
* [shoulda-matchers](https://github.com/thoughtbot/shoulda-matchers) - Shoulda-matchers provides serveral matchers for testing common Rails functionality.
ResponseCodeMatchers provides rspec matchers to match http response code.
* [SimpleCov](https://github.com/colszowka/simplecov) - SimpleCov is a code coverage analysis tool for Ruby.
* [Timecop](https://github.com/travisjeffery/timecop) - A gem providing "time travel" and "time freezing" capabilities, making it dead simple to test time-dependent code.
* [VCR](https://github.com/vcr/vcr) - Record your test suite's HTTP interactions and replay them during future test runs for fast, deterministic, accurate tests.

### Security
* [brakeman](https://github.com/presidentbeef/brakeman) - Brakeman is a static analysis tool which checks Ruby on Rails applications for security vulnerabilities.
* [bundle-audit](https://github.com/rubysec/bundler-audit) - bundler-audit is a patch-level verification tool for Bundler which checks for vulnerable versions of gems and insecure gem sources.
* [Secure Headers](https://github.com/twitter/secureheaders) -  Secure Headers will automatically apply several headers that are related to security.

## Production
* [Capistrano](https://github.com/capistrano/capistrano) - Remote multi-server automation tool.

* [Rack Attack](https://github.com/kickstarter/rack-attack) - Rack middleware to blocking & throttling.


## Error Logging
* [Rollbar](https://github.com/rollbar/rollbar-gem) - Exception tracking and logging from Ruby to Rollbar.

## Frontend
* [slim]
* [bootstrap]
* [bootstrap-datepicker-rails]
* [select2-rails]
* [croeui]
* [toastr-rails]
* [jsoneditor-rails]
* [richexitor]

