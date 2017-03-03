# rcssoccersim telepítése és beállítása Linuxon
1. Töltsd le és csomagold ki a projektet: 
    https://sourceforge.net/projects/sserver/
2. Töltsd le és telepítsd a Boost libeket: 
    http://www.boost.org/users/download/
3. Álltsd be az rcsservert:  
  1. Lépj be a könyvtárba és futtasd:
  ```
  ./configure  
  make  
  make install  
  ``` 
  Dependenciákat kiírja.  
  > Ha a './configure' lefut, de a 'make' nem akkor a './configure' másodszori lefuttatása segíthet.
4. Futtasd:

  ``` 
  sudo apt-add-repository ppa:gnurubuntu/rubuntu   
  ``` 
  majd  
  ``` 
  sudo apt-get update  
  ```
5. Futtasd:
```
sudo apt-get update rssmonitor
```
aminek kell egy env_variable: `export RCSSMONITOR='/usr/bin/rcssmonitor'`

Ha az rcsserver 'make install'-lal települt akkor az `rcsocceersim` paranccsal bárhonnan indítható a szerver és kliens program is egyszerre.
Egy szimulált környezetben való játékra ad lehetőséget.
