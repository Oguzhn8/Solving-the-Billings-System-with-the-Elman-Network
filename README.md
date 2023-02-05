# Solving-the-Billings-System-with-the-Elman-Network
## Elman Network
An Elman network is a three-layer network with the addition of a set of context units. The middle (hidden) layer is connected to these context units fixed with a weight of one. At each time step, the input is fed forward and a learning rule is applied. The fixed back-connections save a copy of the previous values of the hidden units in the context units (since they propagate over the connections before the learning rule is applied). Thus the network can maintain a sort of state, allowing it to perform such tasks as sequence-prediction that are beyond the power of a standard multilayer perceptron. Below is the structure of the Elman network:
![image](https://user-images.githubusercontent.com/78887209/216810960-32e71c83-2b53-41e2-abf5-a6f8cdce2d4a.png) </br>
Elman network are also known as "Simple recurrent networks" (SRN). The basic equations of the Elman network are as follows: </br>
![image](https://user-images.githubusercontent.com/78887209/216811031-eb90fddc-b692-4875-8be8-f35f050834eb.png) </br>
where </br>
![image](https://user-images.githubusercontent.com/78887209/216811049-984e1465-875a-4bc3-ab00-65bb9e73a5b0.png)
### Problem 
In this question, the solution of the following equation expressing the Billings system will be tried to be solved with the Elman Network. </br>
![image](https://user-images.githubusercontent.com/78887209/216811180-9d8e8329-9ab5-48fa-9706-a6fbd3634696.png) </br>
The output of the data set created with the help of the Billing system equation is given below. </br>
![image](https://user-images.githubusercontent.com/78887209/216811231-3bc65eeb-cab5-4b34-822e-c5fdcdac839b.png)
While designing the Elman mesh, y(k) values were taken as output and y(k-1) and y(k-2) values were taken as inputs. Considering the range of values in the data set, the tanh function may be more appropriate as an activation function. Initial weights were randomly generated between 0.5 and -0.5 values. While designing the network, it was decided to use one hidden layer and 8 neurons were used in the relevant layer. 
### Results
The training and testing process results can be viewed below: </br>
![image](https://user-images.githubusercontent.com/78887209/216811514-7cc0861e-ff68-4f42-b7ae-eba9b90f5e98.png) </br>
On the other hand, the estimation outputs of the model and the billing system outputs are shown below: </br>
![image](https://user-images.githubusercontent.com/78887209/216811578-ea3afeb2-5897-4342-8499-c6e67c7c3048.png)
### Further Readings
https://andy-nguyen.medium.com/recurrent-neural-networks-part-1-bf747e07e7dd
