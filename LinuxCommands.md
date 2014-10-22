


### Base64 encoding

   * To output file
   
     * openssl base64 -in /path/to/infile> -out /path/to/outfile

   * Copy to clipboard
      * openssl base64 < path/to/infile | tr -d '\n' | pbcopy 
      
       or 

      * cat path/to/infile | openssl base64 | tr -d '\n' | pbcopy


### Using gnu parallel

* In the command below, change the column separator used in the input file, and the number of arguments to be passed {1} {2} ... as applicable

      * cat path/to/infile | parallel --jobs 4 --colsep '/' /path/to/job/to/be/run/in/parallel {1} {2} 
   
