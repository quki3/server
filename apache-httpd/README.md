# apache
## documentation
<a href="https://archive.apache.org/dist/httpd/docs/httpd-docs-2.4.16.en.pdf">pdf oficial</a>
<a href="https://httpd.apache.org/docs/2.4/">doc oficial</a>
## requeriment 
<sub> the following requeriment exist for building Apache httpd</sub>
1. - APR and APR-Util check if you distro have already installed this
   - `dpkg -l | grep libapr`
   - `dpkg -l | grep libaprutil`
2. - Perl-Compatible Regular Expressions Library (PCRE) check if exist
   - install `sudo apt-get install libpcre3 libpcre3-dev`
3. - dowload
4. - extract
5. - configuring
        - <sub>This is not necessary for official releases.</sub>
        - To configure the source tree using all the default options, simply type ./configure.
                - if you have this error `apr not found`
                - do this
```bash
               

In the directory where you have installed the apache httpd distribution there is a directory that is called /srclib

You cd into that directory cd /srclib. Make sure you are in that folder. Now open your browser and go to http://apr.apache.org/download.cgi and download the apr-*.tar.gz files into this directory.

wget <link>

Unzip and extract them into srclib directory after extracting make sure you rename the apr-* directories to just "apr" and "apr-util", respectively. For example:

mv apr-1.6.5 apr
mv apr-util-1.6.1 apr-util

Now, it should read the .apr files from that folder. After that it will ask for apr-util too, make sure you follow the same procedure.

Hope this helps!

          ```
