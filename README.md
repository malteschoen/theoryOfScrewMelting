# theoryOfScrewMelting

## Melting capacities at different screw diameters for different (fixed!) melting lengths and different melting fluxes

### Table 1: Melting fluxes as determined in the screw simulator

| Material | Melting flux   [kg/(m²*s)] | Melting flux   [(kg/h)/cm²)] |  Examples 
| ----------- | ----------- | ----------- |
| poorly melting | 0.15 |  0.05 | ABS, HIPS, high-viscosity PC |
| average | 0.3  | 0.01 | LLDPE |
| nicely melting |  0.45 | 0.16 | LDPE, low-viscosity PC | 

Melting fluxes are taken from Altınkaynak's dissertation [1]

### 

Screw throughputs are assumed to follow this formula (with throughput in kg/h and diameter in centimetres!), valid for 100 rpm.
```math
\dot{m}=\frac{2}{3}\cdot D^{2.7}
```

The melting surface is assumed to follow this formula (with the length L expressed in multiples of D, e.g. 10 D). Square brackets indicate the contribution of the diameter, regular brackets those of the length.  On average 50 % of barrel surface will be in contact with the solids bed.
```math
A_{melt}=0.5 \left [ \pi\cdot D  \right ]\left (L \cdot D   \right ) 
```

### Table 2: 10 diameters of extruder lenght specified for melting 

| Screw diameter   [mm] | Melting Surface   [cm²] | Typical machine throughput   [kg/h] | Melting capacity, poorly melting material   [kg/h] | Melting capacity, average material   [kg/h] | Melting capacity, nicely melting material   [kg/h] |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| 19 | 60 | 3 | :green_circle:3 | :green_circle:6 | :green_circle:9 |
| 30 | 140 | 12 | :red_circle: 7.5 | :green_circle:15 | :green_circle:22.5 |
| 45 | 320 | 40 | :red_circle: 17 | :red_circle:34 | :green_circle:51 |
| 60 | 560 | 85 | :red_circle: 30 | :red_circle:60 | :yellow_circle:90 |
| 90 | 1270 | 250 | :red_circle: 70 | :red_circle:140 | :red_circle:210 |
| 120 | 2260 | 550 | :red_circle: 125 | :red_circle:250 | :red_circle:375 |

### Table 3: 20 diameters of extruder lenght specified for melting 

| Screw diameter   [mm] | Melting Surface   [cm²] | Typical machine throughput   [kg/h] | Melting capacity, poorly melting material   [kg/h] | Melting capacity, average material   [kg/h] | Melting capacity, nicely melting material   [kg/h] |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| 19 | 120 | 3 | :green_circle:6 | :green_circle:12 |:green_circle:18 |
| 30 | 280 | 12 | :green_circle:15 | :green_circle:30 |:green_circle:45 |
| 45 | 630 | 40 | :yellow_circle:34 | :green_circle:68 |:green_circle:102 |
| 60 | 1020 | 85 | :yellow_circle:60 | :green_circle:120 |:green_circle:180 |
| 90 | 2540 | 250 | :red_circle:140 | :yellow_circle:280 |:green_circle:380 |
| 120 | 4520 | 550 | :red_circle:250 | :yellow_circle:500 |:green_circle:750 |

## Literature
[1]  Altınkaynak, Atakan: Three dimensional finite element simulation of polymer melting and flow in a single-screw extruder: optimization of screw channel geometry, Michigan Technological University, Dissertation, 2010 - http://digitalcommons.mtu.edu/etds/346

 
