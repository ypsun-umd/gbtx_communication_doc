# GBTx communication documentation [![Build status](https://travis-ci.com/ypsun-umd/gbtx_communication_doc.svg?master)](https://travis-ci.com/ypsun-umd)
An effort to record GBTx board setups at UMD LHCb group. We also include all
configuration files used for GBT DB/DCB testing.

## Build
This project utilizes the Travis CI to build and release new pdf files on new tags.
Alternatively, one can clone/download this repository and build pdf files locally with:
```
make pdf
```

If it's your first time to build this project, please create a `build`
directory under the project root.

## Configuration files
Below we list usage of some of the configuration files.

* `master.txt`: For DCB master GBTx. We have enabled watchdog and timeout.
* `slave-Tx.txt`: For DCB data GBTxs. We terminate all E-groups with `0x11`.
* `slave-Tx-wrong_termination.txt`: For DCB data GBTxs. We terminate with `0xFF`.
* `slave-Tx-reduced_eports.txt`: For DCB data GBTxs. Only E-group 0-4 are enabled.
