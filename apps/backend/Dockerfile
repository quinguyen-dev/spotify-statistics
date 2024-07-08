FROM rust:buster as base

WORKDIR /backend
RUN cargo init
COPY Cargo.toml /backend/Cargo.toml
RUN cargo fetch
COPY . /backend

FROM base AS development

CMD [ "cargo", "run"]