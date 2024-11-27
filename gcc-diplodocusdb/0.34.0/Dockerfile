FROM ishiko/gcc-ishiko-cpp:0.44.0

WORKDIR /diplodocusdb

ENV DIPLODOCUSDB_ROOT=/diplodocusdb

RUN git clone https://github.com/diplodocusdb/core.git
RUN cd core/build-files/gnumake && make

RUN git clone https://github.com/diplodocusdb/physical-storage.git
RUN cd physical-storage/build-files/gnumake && make

RUN git clone https://github.com/diplodocusdb/embedded-document-db.git
RUN cd embedded-document-db/storage-engine/build-files/gnumake && make
RUN cd embedded-document-db/database/build-files/gnumake && make

WORKDIR /
