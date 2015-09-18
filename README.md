# lp_solve_python_3x
lpsolve python extension for python 2.x and python 3.x. The lpsolve extension is ported to python3.x so that it works on both python2.x and python3.x. 

There are two options to use lpsolve on Python3.x
# Quick Use
1) Download tar ball "lpsolve55-5.5.0.9.linux-x86_64.tar.gz" under "lp_solve_python_3x/extra/Python/dist_python3.4/" which is built on ubuntu14.04 64-bit machine using Python 3.4.0

2) Extract the files and copy the files under "site-packages/" to local python site-packages folder. 

# Build from sources
1) Download lpsolve source code [lp_solve_5.5.2.0_source.tar.gz](http://sourceforge.net/projects/lpsolve/files/lpsolve/5.5.2.0/lp_solve_5.5.2.0_source.tar.gz/download)

2) Extract the archive and copy extra/Python folder into lp_solve_5.5

3) cd lp_solve_5.5/extra/Python/

4) Use following command to install lpsolve extension into site-packages.
    
        $python setup.py install
