FROM ishikocpp/gcc-ishiko:1.0.0

WORKDIR DiplodocusDB

ENV DIPLODOCUSDB=/DiplodocusDB

RUN git clone https://github.com/DiplodocusDB/Core.git
RUN cd Core/Makefiles/GNUmakefile && make
