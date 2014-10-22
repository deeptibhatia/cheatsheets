


### Base64 encoding

  * From/to file
    openssl base64 -in <infile> -out <outfile>

  * Copy to clipboard
    openssl base64 < path/to/infile | tr -d '\n' | pbcopy 
    or 
    cat path/to/infile | openssl base64 | tr -d '\n' | pbcopy

