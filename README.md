# k8s-check-certificate-chains

Ingress/nginx does not like silly certificates, therefore I created two scripts to find wrong ones.
The script get-all-k8s-certificates.sh retrieves all certificates from kubernetes, and the
check-certificate-chains.sh script verifies the chain's are complete and in proper ordering.

Added md5 hash check on crt and key file to verify the two belong to each other.

The check-certificate-chains.sh just reports on WRONG certificates. Run with "-v" option to also show OK's.

31/7/2018 Thijs Kaper.

https://github.com/atkaper/k8s-check-certificate-chains

