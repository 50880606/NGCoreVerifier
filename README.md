# NGCoreVerifier

We provide an instantiated model with 2 consumers and 3 producers, along with a single property to give an idea of our NGCoreVerifier. Upon accpetance, we will release the full model, a list of all properties we have tested, as well as the model generator to allow instantiation of arbitrary number of configurable NFs to a model.  

The provided property produces a counterexample which represends a Confused Producer Attack. 

## Perform bounded model checking
To run nuXmv:

```
nuXmv -int
```

Then in nuXmv terminal:
```
reset
read_model -i NGCoreVerifier.smv
go_bmc
check_ltlspec_bmc -k 20 # check the property with ltl up to a bound of 20 transitions
```
