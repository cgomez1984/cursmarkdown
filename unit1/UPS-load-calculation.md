# UPS load calculation

The maximum load that a **UPS** can support is measured in **VA** (volt-amperes) and is the apparent power (S), you can see it in any web store or in the image of the UPS on its back; the apparent power ( **S** ), is the vectorial sum of the power:

- **really necessary** for the computer. It is called **active power** ( **P** ). It is measured in watts ( **W** )
- and the power **not used** by the computer but that has been generated in the power supply due to the formation of the electric and magnetic fields of its components. Called **reactive power** ( **Q** ), it is measured in reactive volt-amperes (var).

The **apparent power** ( **S** ), is measured in **VA** (volt-amperes) which is a vectorial sum of the powers (P and Q), somewhat complex to calculate, it can be calculated with the efficiency value (%) of the power supply and its rated power (W). There are various procedures depending on the data we have.

On the other hand, in alternating current it is very easy to know the apparent power if we know the intensity consumed by a device, simply apparent power = Intensity \* network voltage, that is, S = I \* **230** .

## Procedures for calculation 

As always, we have always known data: **230V** , which is the official voltage value of Spain.

All procedures include **S <sub><font style="vertical-align: inherit;">calculated </font></sub>** is the apparent power needed to run the computer, but **only the computer** . As the computer has other peripherals (monitor, external drives, printer,...), it is necessary to estimate a **safety margin for the electrical consumption** of these peripherals. In our case, we estimate to increase the maximum power of the UPS by 30% and it will be the estimated apparent power **S <sub><font style="vertical-align: inherit;">estimated </font></sub>** . S result, <sub><font style="vertical-align: inherit;">With the estimated </font></sub> would only suffice to search for the UPS with a load equal to or greater than the <sub><font style="vertical-align: inherit;">estimated </font></sub> it S.

Therefore, UPS Power >= S <sub><font style="vertical-align: inherit;">estimated </font></sub> , where S <sub><font style="vertical-align: inherit;">estimated </font></sub> \= S <sub><font style="vertical-align: inherit;">calculated </font></sub> \+ (S <sub><font style="vertical-align: inherit;">calculated </font></sub> \* 30%)

## DATA: Maximum power (p) consumed by the source

- Data P= **p** and φ = 0.82 (unknown, 82% efficiency is applied as the worst found is φ =0.82).
- Result:

1. S <sub><font style="vertical-align: inherit;">Calculated </font></sub> \= **p** /0.82 VA
2. Estimated increase in consumption by 30% by peripherals; S <sub><font style="vertical-align: inherit;">Estimated </font></sub> \= <sub><font style="vertical-align: inherit;">Calculated </font></sub> S \* 1.30
3. S <sub><font style="vertical-align: inherit;">estimated </font></sub> will be the power from which we can search for a UPS.

**Typical example:** Calculation of the Apparent Power used if a computer consumes a maximum Power of **500W** , we have:

- Data V=230V, **P=500 W** and φ = 0.82 (unknown, 82% efficiency is applied because φ =0.82 is the worst found). .
- Result:

1. S <sub><font style="vertical-align: inherit;">Calculated </font></sub> \= P / 0.82 VA.
2. S <sub><font style="vertical-align: inherit;">Calculated </font></sub> \= 500 / 0.82 VA = 609.76 VA
3. S <sub><font style="vertical-align: inherit;">estimate </font></sub> \= 609.76 \* 1.30;
4. S <sub><font style="vertical-align: inherit;">Estimated </font></sub> \= **792.68 VA**

If there were 700VA, 1000 VA and 1200 VA UPS. The choice would be the **UPS with 1000 VA** as it is the next one above the minimum value (792.68 VA)

## DATA: Power supply current (I)

- Data **I=i** , V=230V
- Result:

1. S <sub><font style="vertical-align: inherit;">calculated </font></sub> \= **i** \* 230 VA
2. Estimated increase in consumption by 30% by peripherals; S <sub><font style="vertical-align: inherit;">Estimated </font></sub> \= <sub><font style="vertical-align: inherit;">Calculated </font></sub> S \* 1.30
3. S <sub><font style="vertical-align: inherit;">estimated </font></sub> will be the power from which we can search for a UPS

**Typical example:** Calculation of the Apparent Power used if a computer consumes a maximum intensity of 2.173 A, we have:

- Datos: **I=2,173A** , V=230V
- Result:

1. S <sub><font style="vertical-align: inherit;">calculated </font></sub> \= i \* 230 VA
2. S <sub><font style="vertical-align: inherit;">Calculated </font></sub> \=2.173 \* 230 = 500 VA.
3. S <sub><font style="vertical-align: inherit;">Estimated </font></sub> \= 500 \* 1.30
4. S <sub><font style="vertical-align: inherit;">estimated </font></sub> \= **650 VA**

If there were 700VA, 1000 VA and 1200 VA UPS. The choice would be the **UPS with 700 VA** as it is the next one above the minimum value (650 VA)