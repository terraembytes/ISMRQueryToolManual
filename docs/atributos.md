# Attributes

*Source: sbf2ismr v22.1.0*

## Signal groups

1. Sig1:

    - **L1CA** for GPS/GLONASS/SBAS/QZSS 
    - **L1BC** for GALILEO 
    - **B1** for BeiDou 

1. Sig2:

    - **L2C** for GPS/GLONASS/QZSS 
    - **L5** for SBAS 
    - **E5a** for*GALILEO 
    - **B2** for BeiDou 

1. Sig3:

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

*Averaged C/N0 of the second frequency used for the TEC computation*

*avaliable as:*

```
f2nd_tec_cn0
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
*Correction to total S4*

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

*S4 corrected*


  <math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mstyle displaystyle="true" scriptlevel="0">
    <mrow data-mjx-texclass="ORD">
      <mtable rowspacing=".5em" columnspacing="1em" displaystyle="true">
        <mtr>
          <mtd>
            <mrow data-mjx-texclass="ORD">
              <mo stretchy="false">&#x221A;</mo>
            </mrow>
            <mo stretchy="false">(</mo>
            <mi>s</mi>
            <msup>
              <mn>4</mn>
              <mn>2</mn>
            </msup>
            <mo>&#x2212;</mo>
            <mi>s</mi>
            <mn>4</mn>
            <mn>_</mn>
            <mi>c</mi>
            <mi>o</mi>
            <mi>r</mi>
            <mi>r</mi>
            <mi>e</mi>
            <mi>c</mi>
            <mi>t</mi>
            <mi>i</mi>
            <mi>o</mi>
            <msup>
              <mi>n</mi>
              <mn>2</mn>
            </msup>
            <mo stretchy="false">)</mo>
          </mtd>
        </mtr>
      </mtable>
    </mrow>
  </mstyle>
</math>

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    s4_corrected
    ```

=== "Sig2"

    *as*
    ```markdown
    s4_l2_corrected
    ```
    
=== "Sig3"

    *as*
    ```markdown
    s4_l5_corrected
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

## **Code/Carrier divergence (meters)**

*Average*

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

*Standard deviation*

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

## **Total electron content**
*Tec unit*


*avaliable at:*

=== "TOW"

    *as*
    ```markdown
    tec
    ```

=== "TOW - 45 seconds"

    *as*
    ```markdown
    tec_45
    ```

=== "TOW - 30 seconds"

    *as*
    ```markdown
    tec_30
    ```
    
=== "TOW - 15 seconds"

    *as*
    ```markdown
    tec_15
    ```


*Difference of total electron content*


*avaliable from:*

=== "TOW - 60s to 45s"

    *as*
    ```markdown
    dtec_6045
    ```

=== "TOW - 45s to 30s"

    *as*
    ```markdown
    dtec_4530
    ```

=== "TOW - 30s to 15s"

    *as*
    ```markdown
    dtec_3015
    ```
    
=== "15s to TOW "

    *as*
    ```markdown
    dtec_15tow
    ```

* * *

## **Lock time**

Indicates for how long each satellite’s signal has been continuously tracked
on an antenna and is expressed in *seconds*.

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    locktime_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    locktime_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    locktime_l5
    ```

*On the second frequency used for the TEC computation*

*as*

```
f2nd_tec_locktime

```

* * *




## **SI Index**
 <math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mstyle displaystyle="true" scriptlevel="0">
    <mrow data-mjx-texclass="ORD">
      <mtable rowspacing=".5em" columnspacing="1em" displaystyle="true">
        <mtr>
          <mtd>
            <mstyle displaystyle="false" scriptlevel="0">
              <mfrac>
                <mrow>
                  <mo stretchy="false">(</mo>
                  <mn>10</mn>
                  <mo>&#x2217;</mo>
                  <mi>l</mi>
                  <mi>o</mi>
                  <mi>g</mi>
                  <mn>10</mn>
                  <mo stretchy="false">(</mo>
                  <mi>P</mi>
                  <mi>m</mi>
                  <mi>a</mi>
                  <mi>x</mi>
                  <mo stretchy="false">)</mo>
                  <mo>&#x2212;</mo>
                  <mn>10</mn>
                  <mo>&#x2217;</mo>
                  <mi>l</mi>
                  <mi>o</mi>
                  <mi>g</mi>
                  <mn>10</mn>
                  <mo stretchy="false">(</mo>
                  <mi>P</mi>
                  <mi>m</mi>
                  <mi>i</mi>
                  <mi>n</mi>
                  <mo stretchy="false">)</mo>
                  <mo stretchy="false">)</mo>
                </mrow>
                <mrow>
                  <mo stretchy="false">(</mo>
                  <mn>10</mn>
                  <mo>&#x2217;</mo>
                  <mi>l</mi>
                  <mi>o</mi>
                  <mi>g</mi>
                  <mn>10</mn>
                  <mo stretchy="false">(</mo>
                  <mi>P</mi>
                  <mi>m</mi>
                  <mi>a</mi>
                  <mi>x</mi>
                  <mo stretchy="false">)</mo>
                  <mo>+</mo>
                  <mn>10</mn>
                  <mo>&#x2217;</mo>
                  <mi>l</mi>
                  <mi>o</mi>
                  <mi>g</mi>
                  <mn>10</mn>
                  <mo stretchy="false">(</mo>
                  <mi>P</mi>
                  <mi>m</mi>
                  <mi>i</mi>
                  <mi>n</mi>
                  <mo stretchy="false">)</mo>
                  <mo stretchy="false">)</mo>
                </mrow>
              </mfrac>
            </mstyle>
          </mtd>
        </mtr>
      </mtable>
    </mrow>
  </mstyle>
</math>

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    si_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    si_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    si_l5
    ```

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mstyle displaystyle="true" scriptlevel="0">
    <mrow data-mjx-texclass="ORD">
      <mtable rowspacing=".5em" columnspacing="1em" displaystyle="true">
        <mtr>
          <mtd>
            <mstyle displaystyle="false" scriptlevel="0">
              <mfrac>
                <mrow>
                  <mo stretchy="false">(</mo>
                  <mn>10</mn>
                  <mo>&#x2217;</mo>
                  <mi>l</mi>
                  <mi>o</mi>
                  <mi>g</mi>
                  <mn>10</mn>
                  <mo stretchy="false">(</mo>
                  <mi>P</mi>
                  <mi>m</mi>
                  <mi>a</mi>
                  <mi>x</mi>
                  <mo stretchy="false">)</mo>
                  <mo>&#x2212;</mo>
                  <mn>10</mn>
                  <mo>&#x2217;</mo>
                  <mi>l</mi>
                  <mi>o</mi>
                  <mi>g</mi>
                  <mn>10</mn>
                  <mo stretchy="false">(</mo>
                  <mi>P</mi>
                  <mi>m</mi>
                  <mi>i</mi>
                  <mi>n</mi>
                  <mo stretchy="false">)</mo>
                  <mo stretchy="false">)</mo>
                </mrow>
              </mfrac>
            </mstyle>
          </mtd>
        </mtr>
      </mtable>
    </mrow>
  </mstyle>
</math>

*numerator only (dB)*

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    numerator_si_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    numerator_si_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    numerator_si_l5
    ```
* * *

## **Phase spectral Slope**
*0.1 to 25Hz range (dimensionless)*

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    p_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    p_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    p_l5
    ```

* * *

## **Phase power spectral density**
*1 Hz (rad^2/Hz)*

*avaliable at:*

=== "Sig1"

    *as*
    ```markdown
    t_l1
    ```

=== "Sig2"

    *as*
    ```markdown
    t_l2
    ```
    
=== "Sig3"

    *as*
    ```markdown
    t_l5
    ```

* * *

## **Coordinated Universal Time**
LISN receivers use the UTC time system, so there is a difference of a few seconds between records due to the time difference between the GPS and UTC time system.

*LISN receivers data are avaliable as*

```
time_utc_1
time_utc_2
time_utc_3
time_utc_4
time_utc_5
time_utc_p1
time_utc_p2
time_utc_p3
time_utc_p4
time_utc_p5

```




