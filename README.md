# lp_solve_python_3x
lpsolve python extension for python 2.x and python 3.x. The lpsolve extension is ported to python3.x so that it works on both python2.x and python3.x. 

This project is a rework on lpsolve python 5.5.2.0 from http://sourceforge.net/projects/lpsolve/files/lpsolve/5.5.2.0/lp_solve_5.5.2.0_Python_source.tar.gz/download. The lpsolve avaialble in official site is not compatible with python3.x. 

There are two options to use lpsolve on Python3.x
# Quick Use
1) Download tar ball ["lpsolve55-5.5.0.9.linux-x86_64.tar.gz"] (https://github.com/chandu-atina/lp_solve_python_3x/blob/master/extra/Python/dist_python3.4/lpsolve55-5.5.0.9.linux-x86_64.tar.gz) under lp_solve_python_3x/extra/Python/dist_python3.4/" which is built on ubuntu14.04 64-bit machine using Python 3.4.0

2) Extract the files and copy the files under "site-packages/" to local python site-packages folder. 

# Build from sources
1) Download lpsolve source code [lp_solve_5.5.2.0_source.tar.gz](http://sourceforge.net/projects/lpsolve/files/lpsolve/5.5.2.0/lp_solve_5.5.2.0_source.tar.gz/download)

2) Extract the archive and copy extra/Python folder into lp_solve_5.5

3) cd lp_solve_5.5/lpsolve55 and execute following command

        $ sh ccc (on linux)
        $ sh ccc.osx (on Mac)
    Refer to readme.txt under same folder for more information (lp_solve_5.5/lpsolve55/).

3) cd lp_solve_5.5/extra/Python/

4) change lpsolve55 path in extra/Pythpn/setup.py to point to appropriate directory.
    
        LPSOLVE55 = '../../lpsolve55/bin/ux64'  #change path to reflect appropriate path.
> Note: In my case, I used linux 64 bit machine so folder 'bin/ux64/' created under lpsolve55 directory when executed "sh ccc" command from terminal. The folder contains the lpsolve library files. The LPSOLVE55 path in setup.py should point to the newly generated directory which contains the required lpsolve libraries(liblpsolve55.a).

5) Use following command to install lpsolve extension into site-packages.
    
        $python setup.py install
