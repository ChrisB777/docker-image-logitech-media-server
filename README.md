# Docker Container for Logitech Media Server

This is a Docker image for running the Logitech Media Server package
(aka SqueezeboxServer).

Run Directly:

    docker run -d \
               -p 9000:9000 \
               -p 9005:9005 \
               -p 9090:9090 \
               -p 3483:3483 \
               -p 3483:3483/udp \
               -v <local-state-dir>:/srv/squeezebox \
               -v <audio-dir>:/srv/music \
               larsks/logitech/media-server


