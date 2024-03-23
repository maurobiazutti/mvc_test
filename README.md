# TDD_with_RSpec

## Gems necessárias para testes com RSpec

group :development, :test do

  gem "rspec", "~> 3.13"
  gem "rspec-rails"
  gem 'rspec-core', '~> 3.13'
  gem 'rspec-expectations', '~> 3.13'
  gem 'rspec-mocks', '~> 3.13'
  gem 'rspec-support', '~> 3.13', '>= 3.13.1'

  gem 'factory_bot_rails'
  gem 'faker'

end

## Instale

  bundle install

## Comando para geral estrutura de arquivos para testes

  rails g rspec:install

## Descomentar a linha abaixo no arquivo spec/rails_help.rb

  Rails.root.glob('spec/support/**/*.rb').sort.each { |f| require f }

  Este comando carrega dinamicamente todos os arquivos Ruby dentro do diretório spec/support e seus subdiretórios no contexto de um projeto Rails.

## Comentar a linha abaixo no arquivo spec/rails_help.rb

  # config.fixture_path = Rails.root.join('spec/fixtures')

  Fixtures são dados de exemplo usados em testes para preencher o banco de dados com informações conhecidas antes de executar os testes.
  VAMOS USAR FACTORY_BOT_RAILS


## Configuração das gems

No arquivo `spec/rails_helper.rb` adicione o seguinte código: 


