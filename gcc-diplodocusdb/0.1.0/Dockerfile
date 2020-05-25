FROM ishikocpp/gcc-ishiko:1.0.0

WORKDIR /DiplodocusDB

ENV DIPLODOCUSDB=/DiplodocusDB

RUN git clone https://github.com/DiplodocusDB/Core.git
RUN cd Core/Makefiles/GNUmakefile && make

RUN git clone https://github.com/DiplodocusDB/TreeDB.git
RUN cd TreeDB/Core/Makefiles/GNUmakefile && make
RUN cd TreeDB/XMLTreeDB/Makefiles/GNUmakefile && make

WORKDIR /
