# NGCoreVerifier

To run nuXmv:

```
nuXmv -int
```

Then in nuXmv terminal:
```
reset
read_model -i AC.smv
go_bmc
check_ltlspec_bmc -k 20 # check the property
```
