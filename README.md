# How to run details service

## Prerequisite

* Ruby 2.7

```bash
ruby details.rb 8081
```

## How to run with Docker

```bash
# Build Docker Image for book-details service
docker build -t book-details-ruby .

# Run book-details service on port 8081
docker run -d -it --name book-details-service -p 8081:9080 -e ENABLE_EXTERNAL_BOOK_SERVICE=true book-details-ruby
```
## How to run with Docker Compose

```bash
docker-compose up
```

* Test with path `/details/1` and `/health`
