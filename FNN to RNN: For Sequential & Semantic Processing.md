(FNN - FeedForward Neural Network, RNN - Recurrent Neural Network)
## Base Architecture Of a Neural Network
Input Layer --> Hidden Layer(s) --> Output Layer  


## FNN's way of processing sequential data
Suppose a dataset has ten rows, two columns. One column has textual data and the other has labels. The first row in first column has the text "Eye for an eye makes the whole world blind."

This whole sentence will be fed as first input to the FNN. To processes it, the FNN should be fed the flattened embeddings (vectors) of each word in the sentence. Flattened embeddings mean to sum up the embeddings of all words. Once the total of embeddings i.e. the flattened embedding is fed to the FNN, the further process occurs same as the layer architecture mentioned above, input to hidden layer(s) to output.  

***Key Point**: The flattended embedding for "Eye for an eye makes the whole world blind." and "The whole eye world makes eye for an blind." would be same. Because the FNN does not have memory, it does not store the order and context of the elements in the sequence.*

## RNN's way of processing sequential data
The advantage that RNN has is of memory. RNNs use memory to store order and context of each word in the sentence. So, for the sentence "Eye for an eye makes the whole world blind." the RNN's first hidden layer will process it as follows:  

	Eye --> (Vector for Context & Position of 'Eye') = first hidden state --> h1  
	for --> (Vector for Context & Position of 'for') + h1 = second hidden state --> h2  
	an --> (Vector for Context & Position of 'an') + h2 = third hidden state --> h3  
	...  
	...  
	blind --> (Vector for Context & Position of 'blind') + h8 = ninth hidden state --> h9 --> output of first row
