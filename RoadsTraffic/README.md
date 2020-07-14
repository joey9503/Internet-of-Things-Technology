# lab-2 report
## FlowChart
![flow-chart](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqrs56w3lj30yl08ijsw.jpg)
## Experiment 1
Maximum number of cars equals to 20: No traffic jam.
![20-cars](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqnmdms3wg30rv0gre81.gif)
<br></br>
Maximum number of cars equals to 50: Minor traffic jam.
![50-cars](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqo5v0xi2g30rv0gru0z.gif)
Clearly, the third intersection(look down from the top) has a minor traffic jam.
<br></br>
Maximum number of cars equals to 80: Heavy traffic jam.
![80-cars](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqosbkkh0g30rx0gru0x.gif)
From this graph, there is a heavy traffic jam in the second intersection.<br></br>
## Experiment 2
From graph above, cars are only allowed to turn right in every intersection and will turn around at the end of the road. As described in the section "FlowChart", there is only one `carSource` in the whole model and there is on `CarDispose` so that the number of cars is fixed.
## Experiment 3
The master and slave could be set with `probability`:  
![prob](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqrzjm77xj30e6051t8p.jpg)
<br></br>
Compared with experiment 1, 3 experiments are going to be conducted:  
`MaximumCars = 20`  
`probability = 0.6` (probability of the side road is 0.6 and the probability of the  middle road is 0.4.)
![prob-cars-20](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqv6fvhpjg30rx0grx6j.gif)
Obviously, compared to the counterpart, there is a minor traffic jam between the first intersection and the second intersection.
<br></br>
`MaximumCars = 50`  
`probability = 0.7`
![prob-cars-50](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqvepu5xig30rx0grb2a.gif)
The site of traffic jam is basically same with the `MaximumCars = 20`. The reasonable explanation is that when the cars at the first intersection, as the probability of side road is greater than the middle road's, marjority of cars choose to turn right, which could slow down cars behind. It can be deduced that when `MaximumCars = 80` and `probability = 0.7` the model has a similar behavior.
<br></br>
`MaximumCars = 80`  
`probability = 0.7`
![prob-cars-80](https://tva1.sinaimg.cn/large/007S8ZIlgy1ggqvuk6snig30rx0grb2a.gif)
Just as the prediction above, the traffic jam is much more serious than its counterpart.
## Summary
In this lab work, I knew:
1. How to add cars and plan a route for them.
2. How to assign different probability to control the traffic.  

The traffic is not handled well right now so there are many serious traffic jam in different intersection. It might needs traffic light to control the traffic in the intersection.