# DSPractical3
Steps:

1. Download openmpi-4.1.4.tar.bz2 from http://www.open-mpi.org in a folder sayLP5.
2. 
	- sudo apt-get update
	- sudo apt install gcc 

3. tar -jxf openmpi-4.1.4.tar.bz2

4. Configure, compile and install by executing the following commands
  -	./configure --prefix=$HOME/opt/openmpi
	- make all
	- make install

5. Update the PATH and LD_LIBRARY_PATH environment variable using
	- echo "export PATH=\$PATH:\$HOME/opt/openmpi/bin" >> $HOME/.bashrc
	- echo" export LD_LIBRARY_PATH=\$LD_LIBRARY_PATH:\$HOME/opt/openmpi/lib" >> $HOME/.bashrc

6. mpicc Array.c
7. mpirun -np 4 ./a.out
