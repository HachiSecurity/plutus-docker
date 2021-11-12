FROM haskell:8.10.4
RUN apt-get update && \
    apt-get install -y libsodium-dev
COPY cabal.project /cabal.project
RUN cabal update && cabal install plutus-core
