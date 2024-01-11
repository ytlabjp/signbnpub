# SiGN-BN Public Repository
This Github repository is for public repository for old SiGN-BN binaries.
The official web site is https://sign.hgc.jp/signbn/ . 
Visit there for the latest information.

SiGN-BN Rel. 1 series such as HC+BS 1.8.3 and NNSR 0.16.8 are no longer being updated.
I recommend using SiGN-BN 2 series or INGOR.

## About license
The SiGN-BN executable binaries are available under the following terms.

Use Restrictions

You may not:
- modify, translate, reverse engineer, decompile, disassemble or otherwise attempt to reconstruct or discover the source code from the binaries of the Software, except to the extent applicable laws specifically prohibit such restriction.
- create derivative works based on the software (e.g. incorporating the software in a commercial product or service without a proper license).
- copy the software.
- rent, lease, sublicense, convey, distribute or otherwise transfer rights to the software.
- remove any product identification, copyright, proprietary notices or labels from the software.

Limitations of Liability

In no event shall the initial developers or copyright holders be liable for any damages whatsoever, including - but not restricted to - lost revenue or profits or other direct, indirect, special, incidental or consequential damages, even if they have been advised of the possibility of such damages, except to the extent invariable law, if any, provides otherwise.

No Warranty
The software and this license document are provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.

The SiGN-BN binaries include SFMT Copyright © 2006, 2007 Mutsuo Saito, Makoto Matsumoto and Hiroshima University, & Copyright © 2012 Mutsuo Saito, Makoto Matsumoto, Hiroshima University and The University of Tokyo.

Please cite our publications (see PUBLICATIONS in the web site) when you publish your results.


## Binaries
### SiGN-BN HC+BS rel. 1.8.3 binary for Linux x86-64 (signbn.1.8.3.gz)
- Gzipped executable binary compiled for Linux x86-64.
- The required libraries are statically linked. Therefore, this should work on every general linux x86-64 system.
- Confirmed to work on CentOS 8 with AMD EPYC 7502P, CentOS 7 with Intel(R) Xeon(R) Gold 6154.

### SiGNB-BN NNSR rel. 0.16.8 binary for Linux x86-64 (signbnnnsr.0.16.8.gz)
- Gzipped executable binary compiled for Linux x86-64.
- This is parallelized with Open MPI 4.1.0. You require Open MPI installed on your system and to execute this via mpirun command.
- Set the Open MPI library path to the environment variable LD_LIBRARY_PATH if you have an error about the missing library file.
- FYI: Using a server with Intel Xeon Platinum 8160 (2.1GHz) CPUs and 64 processes, it takes 1 hour and a half to finish the network estimation with "-T 15000" option for GN-10k-500.edf.txt, which can be downloaded from the web site.

Copyright (C) 2024 Yoshinori Tamada
