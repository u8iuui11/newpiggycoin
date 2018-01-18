Oinkcoin Specs & Information README (or maybe dont)
====================================================

Oinkcoin uses Proof of Listening (PoL), a NEW way to "Mine" which uses your devices audio output to ommit certain sound effects. If volume is muted or not above a certain % then no shares will be submitted. The bigger and better the audio devices used are, the more shares will be submitted.

 - 150 second block targets
 - 800,000,000 total coins
 - No Premine, we aren't hogs here ;)
 - Block reward will use "Shell Distribution"
 

Getting Started
----------------
### How to build OinkCoin

    sudo apt-get install build-essential \
                         libssl-dev \
                         libdb5.1++-dev \
                         libboost-all-dev \
                         libqrencode-dev \
                         libminiupnpc-dev

    cd src/
    make -f makefile.unix USE_UPNP= USE_IPV6=1 USE_QRCODE=1

### Quickstart for Linux Users

    cd ~
    sudo apt-get install build-essential \
                         libssl-dev \
                         libdb5.1++-dev \
                         libboost-all-dev \
                         libqrencode-dev \
                         libminiupnpc-dev \
                         libcurl4-openssl-dev \
                         qt4*
    git clone https://github.com/u8iuui11/oinkcoin.git
    cd newpiggycoin
    qmake USE_UPNP=0 USE_IPV6=1 USE_QRCODE=1 && make
    
For more information and options, please look at doc/build-unix.md.
