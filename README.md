Small demo showing how only the last `addCustomCode` call is honoured by the game.

The Kushan Probe's `.ship` file has two calls, one to `script_a`'s `A` function, and a second to `script_b`'s `B` function. Both are on different timings.

Only `B` is called.

Log output:

```
*****---- CommandConstructionComplete : buildingShip=Kus_Carrier, builtItem=Kus_Probe, buildType=1
CALL FROM UPDATE B AT 26.69987869262695
CALL FROM UPDATE B AT 28.74984741210938
CALL FROM UPDATE B AT 30.7998161315918
CALL FROM UPDATE B AT 32.84978485107422
CALL FROM UPDATE B AT 34.89975357055664
CALL FROM UPDATE B AT 36.94972229003906
CALL FROM UPDATE B AT 38.99969100952148
CALL FROM UPDATE B AT 41.04965972900391
CALL FROM UPDATE B AT 43.09962844848633
**** StatusShipDestroyed: shipName =Kus_Probe, and code = -1
```
