# How to run details service

## Prerequisite

* Ruby 2.7

```bash
ruby details.rb 8081
```

## How to run with Docker

```bash
# Build Docker Image for book-details service
docker build -t ruby-book-details .

# Run book-details service on port 8081
docker run -d -it --name ruby -p 8081:8081 -e ENABLE_EXTERNAL_BOOK_SERVICE=true book-details-ruby
```

* Test with path `/details/1` and `/health`
