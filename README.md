# processLCM_RSI
LCM processing and analysis of RSI reconstructed data

Linux Installation:

If files needed and Matlab Runtime are installed within a user’s home directory, no root/superuser permissions should be required. Local installation packages (which include the Matlab Runtime) are located at  https://pitt.box.com/s/sedtq105ehmve7ni8cd5ty8h7zjk5pwp 

> ./lcmRSI_localInstaller.install &
and follow directions (the default installation directories require root).

Help:

> lcm_rsi -help

Usage:

> lcm_rsi &

OR 

> lcm_rsi TimeDomainDataMatlabFile NoOfCPUsToUse savePicsTrueFalse lcmBasisSet &


-TimeDomainDataMatlabFile contains the time domain (TD) spectral data to be processed (e.g.siarrayDATA.mat or siarrayDATA_SCT.mat). Use relative or absolute path if not in CWD

-NoOfCPUsToUse is the number of parallel threads used for processing by LCM

-savePicsTrueFalse: To generate pics, enter 1. If no connection to the X server, enter 0 here.

-lcmBasisSet used by LCM. Use relative or absolute path if not in CWD. For Hadamard scans using more than one set, select the set corresponding to each slice, starting with most inferiorly positioned slice to most superior, or/and edit LCMparams.txt file once generated.
