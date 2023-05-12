# Attributes

*Source: sbf2ismr v22.1.0*

* * *
## **GPS Week Number**

*available as:*

> wn

* * *

## **GPS Time of Week (seconds)**

*available as:*

>tow

* * *

## **Satellite identification**

*available as:*

>svid 
 
    1-37: Pseudorandom noise (PRN) number for GPS satellites

    38-61: Slot number for GLONASS satellites (with an offset of 37)

    71-106: PRN number for GALILEO satellites (with an offset of 70)

    120-138: PRN number for SBAS satellites

* * *

## **Value of the RxState field of the ReceiverStatus SBF block**

*avliable as:*

>sbf_block

* * *

## **Azimuth (degrees)**
It indicates the direction of the projection of the line-of-sight onto the local horizontal plane measured from the geographic North
positive to the East.

*avaliable as:*

>azim

* * *

## **Elevation (degrees)**
It defines the angle between the local horizontal plane and the direction to the satellite.

*avaliable as:*

>elev

* * *

## **Average signal C/N0 over the last minute (dB-Hz)**
Carrier-to-Noise Ratio

*avaliable at:*

- GPS/GLONASS/SBAS/QZSS **(L1CA)**
- GALILEO **(L1BC)**
- BeiDou **(B1)**

*as*
>avg_cn0_l1

*avaliable at:*

- GPS/GLONASS/QZSS **(L2C)**
- SBAS **(L5)**
- GALILEO **(E5a)**
- BeiDou **(B2)**

*as*
>avg_cn0_l2

*avaliable at:*

- GPS/QZSS **(L5)**
- GALILEO **(E5b)**

*as*
>avg_cn0_l5

* * *

## **Total S4 on signal (dimentionless)**

*avaliable at:*

- GPS/GLONASS/SBAS/QZSS **(L1CA)**
- GALILEO **(L1BC)**
- BeiDou **(B1)**

*as*
>s4

*avaliable at:*

- GPS/GLONASS/QZSS **(L2C)**
- SBAS **(L5)**
- GALILEO **(E5a)**
- BeiDou **(B2)**

*as*
>s4_l2

*avaliable at:*

- GPS/QZSS **(L5)**
- GALILEO **(E5b)**

*as*
>s4_l5

* * *

## **Correction to total S4 on signal (thermal noise component only) (dimensionless)**

*avaliable at:*

- GPS/GLONASS/SBAS/QZSS **(L1CA)**
- GALILEO **(L1BC)**
- BeiDou **(B1)**

*as*
>s4_correction

*avaliable at:*

- GPS/GLONASS/QZSS **(L2C)**
- SBAS **(L5)**
- GALILEO **(E5a)**
- BeiDou **(B2)**

*as*
>s4_correction_l2

*avaliable at:*

- GPS/QZSS **(L5)**
- GALILEO **(E5b)**

*as*
>s4_correction_l5

* * *






