# Attributes

*Source: sbf2ismr v22.1.0*

## Signal groups

Sig1:

- **L1CA** for GPS/GLONASS/SBAS/QZSS 
- **L1BC** for GALILEO 
- **B1** for BeiDou 

Sig2:

- **L2C** for GPS/GLONASS/QZSS 
- **L5** for SBAS 
- **E5a** for*GALILEO 
- **B2** for BeiDou 

Sig3:

- **L5** for GPS/QZSS 
- **E5b** for GALILEO 


* * *
## **GPS Week Number**

*available as:*


```
wn

```

* * *

## **GPS Time of Week (seconds)**

*available as:*


```

tow

```

* * *

## **Satellite identification**

*available as:*


```

svid

```
 
>1-37: [PRN]("Pseudorandom noise") number for GPS satellites

>38-61: Slot number for GLONASS satellites (with an offset of 37)

>71-106: PRN number for GALILEO satellites (with an offset of 70)

>120-138: PRN number for SBAS satellites

* * *

## **Value of the RxState field of the ReceiverStatus SBF block**

*avliable as:*


```

sbf_block

```

* * *

## **Azimuth (degrees)**
It indicates the direction of the projection of the line-of-sight onto the local horizontal plane measured from the geographic North
positive to the East.

*avaliable as:*

```

azim

```

* * *

## **Elevation (degrees)**
It defines the angle between the local horizontal plane and the direction to the satellite.

*avaliable as:*

```

elev

```

* * *

## **Average signal C/N0 over the last minute (dB-Hz)**


Carrier-to-Noise Ratio

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    avg_cn0_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    avg_cn0_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    avg_cn0_l5
    ```



* * *

## **Total S4 on signal (dimentionless)**

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    s4
    ```

=== "Sig2"

    *as*
    ```markdown
    s4_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    s4_l5
    ```
* * *

## **Correction to total S4 on signal**
*Thermal noise component only (dimensionless)*

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    s4_correction
    ```

=== "Sig2"

    *as*
    ```markdown
    s4_correction_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    s4_correction_l5
    ```

* * *

## **Phi on signal**


### Phi01

- 1 second phase sigma (radians)

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    phi01|1

    ```

=== "Sig2"

    *as*
    ```markdown
    phi01_l2

    ```
    
=== "Sig3"

    *as*
    ```markdown
    phi01_l5
    ```


### Phi03


- 3 second phase sigma (radians)

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    phi03|1

    ```

=== "Sig2"

    *as*
    ```markdown
    phi03_l2

    ```
    
=== "Sig3"

    *as*
    ```markdown
    phi03_l5
    ```

### Phi10

- 10 second phase sigma (radians)

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    phi10|1

    ```

=== "Sig2"

    *as*
    ```markdown
    phi10_l2

    ```
    
=== "Sig3"

    *as*
    ```markdown
    phi10_l5
    ```

### Phi30 

- 30 second phase sigma (radians)

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    phi30|1

    ```

=== "Sig2"

    *as*
    ```markdown
    phi30_l2

    ```
    
=== "Sig3"

    *as*
    ```markdown
    phi30_l5
    ```


### Phi60

- 60 second phase sigma (radians)

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    phi60|1

    ```

=== "Sig2"

    *as*
    ```markdown
    phi60_l2

    ```
    
=== "Sig3"

    *as*
    ```markdown
    phi60_l5
    ```

* * *

## **Average of code/carrier divergence (meters)**

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    avgccd_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    avgccd_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    avgccd_l5
    ```

* * *

## **Standard deviation of code/carrier divergence (meters)**

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    sigmaccd_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    sigmaccd_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    sigmaccd_l5
    ```

* * *


