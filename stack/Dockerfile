FROM haskell:8.10.7
ARG resolver=lts-17.14.plutus.yaml
RUN apt-get update && \
    apt-get install -y libsodium-dev
COPY ${resolver} /${resolver}
RUN stack install --system-ghc --resolver=${resolver} plutus-core
