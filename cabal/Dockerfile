FROM haskell:8.10.4
RUN apt-get update && \
    apt-get install -y libsodium-dev
COPY cabal.project /cabal.project
# use v1-install to install globally
RUN cabal update && cabal v1-install \
    ouroboros-network \
    cardano-ledger-shelley cardano-api \
    plutus-core plutus-chain-index-core plutus-ledger plutus-tx
