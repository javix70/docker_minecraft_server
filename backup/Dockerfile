FROM alpine:latest

RUN apk add --no-cache git tar bash

COPY backup_restore.sh /usr/local/bin/backup_restore.sh

RUN chmod +x /usr/local/bin/backup_restore.sh

CMD ["sh", "-c", "while true; do /usr/local/bin/backup_restore.sh backup; sleep 120; done"]
#CMD ["sh", "-c", "while true; do echo 'holamundo'; sleep 2; done"]
