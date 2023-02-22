namespace :greeting do
  desc "hello from rake"
  task :hello do
    puts "hello from Rake!"
  end

  desc "hola from rake"
  task :hola do
    puts "hola de Rake!"
  end
end

desc "rake console"
task :console do
end

namespace :db do
  desc "Migrate changes to data"
  task migrate: :environment do
    Student.create_table
  end
  
  desc "seed the database"
  task :seed do
    require_relative('db/seeds.rb')
  end

end

desc "setup the environment"
task :environment do
  require_relative 'config/environment'
end
