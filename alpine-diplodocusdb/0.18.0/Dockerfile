FROM ishiko/alpine-ishiko-cpp:0.20.0

WORKDIR /diplodocusdb

ENV DIPLODOCUSDB_ROOT=/diplodocusdb

RUN git clone https://github.com/diplodocusdb/core.git
RUN cd core/build/gnumake && make

RUN git clone https://github.com/diplodocusdb/physical-storage.git
RUN cd physical-storage/build/gnumake && make

RUN git clone https://github.com/diplodocusdb/embedded-document-db.git
RUN cd embedded-document-db/storage-engine/build/gnumake && make
RUN cd embedded-document-db/database/build/gnumake && make

WORKDIR /
