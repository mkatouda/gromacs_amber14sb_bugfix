# gromacs_amber14sb_bugfix
Bugfix of amber14sb force field of gromacs following webpages:

## Fixing bugs in FF14SB port for Gromacs
http://zhenglz.blogspot.com/2017/05/fixing-bugs-in-ff14sb-port-for-gromacs.html

Add the following two lines in the ffbonded.itp after the 730th lines:   

```
NA  CW  CC  CT       4      180.00     4.60240     2     ;;; HID force field added
NA  CV  CC  CT       4      180.00     4.60240     2     ;;; HID force field added
```

The atom type CV and CW here are similar and share the same parameter value.    

## Install new amber force fields ports in Gromacs
http://zhenglz.blogspot.com/2017/05/install-new-amberff-ports-in-gromacs.html

## Contact
Michio Katouda (katouda@rist.or.jp) 
