# DeFi

This file blockchain-based ledger system with a user-friendly web interface that allows users to send currency.

First, imports and dependancies are loaded.

![Imports and dependencies](Images/1.PNG)

Then a class is created called "Record" that stores sender, receiver, and amount data for use later in the code.

![Record data class](Images/2.PNG)

Next the "Block" class is created that establishes the current block's details including the inputs from "Record" as well as creator ID, the previous block's hash, the timestamp, and the nonce, then hashes these items.

![Block data class](Images/3.PNG)

This is followed by the "Pychain" class that takes in each "Block", establishes proof of work, adds the block to the chain, then verifies and hashes it.

![Pychain data class](Images/4.PNG)

After establishing the above data classes, streamlit code is started and the chain setup function is created and instantiated.

![Streamlit initialization](Images/5.PNG)

Streamlit code is then added for user inputs to enter the fields established in the "Record" class, as well as a button that initializes the addition of a new block in the chain.

![Streamlit new block inputs](Images/6.PNG)

Finally the code adds a dataframe to track the chain and a difficulty slider to adjust hash difficulty on a sidebar along with a dropdown that allows blocks to view them individually.

![Streamlit outputs](Images/7.PNG)

When app is run through streamlit in the command line it produces the following interface:

![Streamlit interface](Images/8.PNG)
