# **cmpsc-90ba-docker-image**
## _Packages that the Professor requested:_
 * Upgrade otter-grader=2.1.1 to 2.2.5 (completed) 
***

### **Ubuntu Packages:**
``` Dockerfile
 apt-get install -y \
        libxtst-dev \
        zsh \
        powerline \
        fonts-powerline \
        less \
        bsdmainutils \
        pv
```
***
### **Jupyter labextensions Installations:**


``` Dockerfile
 jupyter contrib nbextension install --sys-prefix 
 jupyter nbextension install nbzip --py --sys-prefix  
 jupyter nbextension install rise --py --sys-prefix 
 jupyter nbextension install --py hide_code --sys-prefix 
``` 
#### _Labextensions that had to be enabled:_
 * toc2/main --sys-prefix 
 * rise --py --sys-prefix
 * nbzip --py --sys-prefix 
 * table_beautifier/main --sys-prefix 
 * toggle_all_line_numbers/main --sys-prefix
 * jupyter serverextension enable nbzip --py --sys-prefix
 * jupyter nbextensions_configurator enable --sys-prefix 
 * jupyter nbextension enable --py hide_code --sys-prefix 
 * jupyter serverextension enable --py hide_code --sys-prefix



***

### **Pip Packages:**
``` Dockerfile
    pip install \
        pandas \
        cvxpy \
        nltk \
        quandl \ 
        altair vega_datasets \
        otter-grader==2.2.5 \
        ipywebrtc \
        ipympl \
        #ipywidgets \
        matplotlib \
        jupyter_bokeh \
        nbdime \
        jupytext --upgrade \
        jupyterlab_vim \
        jupyterlab_widgets \
        ipympl \
        jupyter \
        jupyterlab \
``` 
  * pip install --upgrade jupyterlab-git
  * pip install nbzip
  * pip install --pre rise
  * pip install hide_code
***
### **Conda Packages:**
``` Dockerfile
 npm install -g npm@latest 
 npm install -g codemirror 
```


