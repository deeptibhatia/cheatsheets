


### Base64 encoding

   * To output file
   
     * openssl base64 -in /path/to/infile> -out /path/to/outfile

   * Copy to clipboard
      * openssl base64 < path/to/infile | tr -d '\n' | pbcopy 
      
       or 

      * cat path/to/infile | openssl base64 | tr -d '\n' | pbcopy

