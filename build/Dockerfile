FROM ubuntu:focal

COPY ${PWD}/deb/*.deb /
 
COPY ${PWD}/install.sh /install.sh
 
RUN chmod +x /install.sh && /install.sh

COPY ${PWD}/rtpengine.conf /rtpengine.conf
COPY ${PWD}/rtpengine.sh /rtpengine.sh
RUN chmod 755 /rtpengine.sh

CMD /rtpengine.sh