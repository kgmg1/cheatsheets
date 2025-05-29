# cheatsheets
echo -n | openssl s_client -showcerts -connect <hostname>:<port> | sed -ne '/-BEGIN CERTIFICATE-/,/-END CERTIFICATE-/p' > server_chain.pem
