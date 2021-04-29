# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION

DECIDIM_VERSION = { git: "https://github.com/decidim/decidim", branch: "develop" }

gem "decidim", DECIDIM_VERSION
#gem "decidim-conferences", DECIDIM_VERSION
#gem "decidim-consultations", DECIDIM_VERSION
gem "decidim-elections", DECIDIM_VERSION
#gem "decidim-initiatives", DECIDIM_VERSION
#gem "decidim-templates", DECIDIM_VERSION

gem "uglifier", ">= 1.3.0"
gem "wicked_pdf"
gem "wkhtmltopdf-binary"

gem "faker", "~> 2.14"

gem "puma"

gem "webpacker", "6.0.0.beta.7"

group :development, :test do
  gem "byebug", platform: :mri
end

group :development do
  gem "decidim-dev", DECIDIM_VERSION
  gem "letter_opener_web", "~> 1.4.0"
  gem "listen", "~> 3.1.0"
  gem "spring"
  gem "spring-watcher-listen", "~> 2.0.0"
  gem "web-console"
end

group :production do
  gem "fog-aws"
  gem "lograge"
  gem "sendgrid-ruby"
  gem "sentry-ruby"
  gem "sentry-rails"
end
