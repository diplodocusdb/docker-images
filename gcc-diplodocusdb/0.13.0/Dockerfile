FROM ishiko/gcc-ishiko-cpp:0.22.0

WORKDIR /diplodocusdb

ENV DIPLODOCUSDB=/diplodocusdb

RUN git clone https://github.com/diplodocusdb/core.git
RUN cd core/build/gnumake && make

RUN git clone https://github.com/diplodocusdb/tree-db.git
RUN cd tree-db/core/build/gnumake && make
RUN cd tree-db/xml-tree-db/build/gnumake && make

WORKDIR /
