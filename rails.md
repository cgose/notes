Ruby on Rails
====================

## Test Environment Setup

> Edit the Gemfile
```ruby
#TODO: insert the code
group :test do
    gem 'shoulda'
    gem 'fabrication'
    gem 'rails-controller-testing'
end
```

> Edit the application.rb file
```ruby
#TODO: insert the code
config.app_generators do |g|
    g.test_framework :test_unit, fixture_replacement: :fabrication
    g.fixture_replacement, dir: "test/fabricators"
end
```

### Fabrications / Fabricators
- Fabricators are created when model generated. The above code sets it up
- It will create the fabricators folder if not already there



# Models

## Making changes to database
```ruby
rake db:schema:load
```
### Generating a model
> The command to generate a model
```ruby
rails generate model Status text:text likes:integer
```

The rails model generator supports the following types:
- integer
- primary_key
- decimal
- float
- boolean
- binary
- string
- text
- date
- time
- datetime

> There is some debate whether to use text versus string

## Migrations
Changes aren't written to the database until the migrations are ran
```ruby
rake db:migrate 
```
This command writes the changes to the database

### Making changes to model
After generating a model with the model generator you can
create a migration to update that model

```ruby
rails generate migration AddCategoryIdToProduct category_id:integer
```
This will generate a new migration that should look like this
```ruby
class AddCategoryIdToProduct < ActiveRecord::Migration
    def change
        add_column :products, :category_id, :integer
    end
end
```
# Controllers

# Views

# Scaffolding

# Testing



