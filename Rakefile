# desc 'outputs hello to the terminal'
# task :hello do
#   puts "hello from Rake!"
# end

namespace :greeting do
  desc "outputs hello from rake"
  task :hello do
    puts "hello from Rake!"
  end

  desc "outputs hola from rake"
  task :hola do
    puts "hola de Rake!"
  end
end

desc "console task"
task :console do
  puts "Make sure you have a 'console' rake task"
end

task :environment do
  require_relative "./config/environment"
end

namespace :db do
  desc "migrate changes to your database"
  task :migrate => :environment do
    Student.create_table
  end

  desc "seed database with dummy data"
  task :seed do
    require_relative "./db/seeds.rb"
  end
end
