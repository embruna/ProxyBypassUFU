# ProxyBypassUFU
Instructions on how to bypass the UFU firewall &amp; use RStudio

TO BY PASS FIREWALL AND LOAD PACKAGES
TURN OFF R

1) Open Terminal and do the following:

export http_proxy=http://proxy.ufu.br:3128
export HTTP_PROXY=proxy.ufu.br:3128

2) Open R and run the following

Sys.setenv(http_proxy="http://proxy.ufu.br:3128")
Sys.getenv("http_proxy")


Often easier to install packages from R rather than RStudio using install.packages("packagename")

SOURCE:  http://braz.blogspot.com.br/2007/07/installing-upgrading-r-thru-http-proxy.html

