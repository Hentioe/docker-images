FROM elixir:1.10.3-slim


RUN apt-get update \
    && apt-get install git build-essential -y\
    && rm -rf /var/lib/apt/lists/* \
    && rm -rf /var/lib/apt/lists/partial/*
RUN mix local.hex --force \
    && mix local.rebar --force


WORKDIR /code


CMD ["iex"]
