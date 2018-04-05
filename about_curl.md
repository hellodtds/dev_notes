#About Curl

##LATEST VERSION

  You always find news about what's going on as well as the latest versions
  from the curl web pages, located at:

        http://curl.haxx.se

##SIMPLE USAGE

  - Get the main page from Netscape's web-server:

        curl http://www.netscape.com/

  - Get the README file the user's home directory at funet's ftp-server:

        curl ftp://ftp.funet.fi/README

  - Get a web page from a server using port 8000:

        curl http://www.weirdserver.com:8000/

  - Get a directory listing of an FTP site:

        curl ftp://cool.haxx.se/

  - Get the definition of curl from a dictionary:

        curl dict://dict.org/m:curl

  - Fetch two documents at once:

        curl ftp://cool.haxx.se/ http://www.weirdserver.com:8000/

  - Get a file off an FTPS server:

        curl ftps://files.are.secure.com/secrets.txt

  - or use the more appropriate FTPS way to get the same file:

        curl --ftp-ssl ftp://files.are.secure.com/secrets.txt

  - Get a file from an SSH server using SFTP:

        curl -u username sftp://shell.example.com/etc/issue

  - Get a file from an SSH server using SCP using a private key to authenticate:

        curl -u username: --key ~/.ssh/id_dsa --pubkey ~/.ssh/id_dsa.pub \
            scp://shell.example.com/~/personal.txt

  - Get the main page from an IPv6 web server:

        curl -g "http://[2001:1890:1112:1::20]/"

## TO DOWNLOAD TO A FILE

  - Get a web page and store in a local file with a specific name:

        curl -o thatpage.html http://www.netscape.com/

  - Get a web page and store in a local file, make the local file get the name
  of the remote document (if no file name part is specified in the URL, this
  will fail):

        curl -O http://www.netscape.com/index.html

  - Fetch two files and store them with their remote names:

        curl -O www.haxx.se/index.html -O curl.haxx.se/download.html
