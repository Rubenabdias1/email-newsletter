# email-newsletter

Zero to Production In Rust's email newsletter project

## Build the container

docker build --tag zero2prod --file Dockerfile .

Since sqlx will check at compile-time:
cargo sqlx prepare --workspace

Running the image:
docker run -p 8000:8000 zero2prod

## Health check

curl -v http://127.0.0.1:8000/health_check
