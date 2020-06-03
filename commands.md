# this script creates a docker volume "certs" containing my LetsEncrypt certificates
# to use the volume, mount it on /etc/letsencrypt/

docker volume create certs
docker run --rm -v certs:/recover -v $(pwd)/certs:/backup ubuntu bash -c "cd recover && tar xvf /backup/certbackup.tar"

# this is to make a backup of the certificate files inside the certs volume
docker run --rm -v certs:/certs -v $(pwd)/certs:/backup ubuntu tar cvf /backup/certbackup.tar /certs
