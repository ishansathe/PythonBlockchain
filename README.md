# PythonBlockchain
 Demonstrating the working and structure of blockchain with python programming language

The base code was referred from the following tutorial:
https://www.tutorialspoint.com/python_blockchain/index.htm

Download and import the code onto JupyterLab (or a similar notebook) in order to make it work

Many changes were made to the code, some were to improve the code, some were to satisify my interest, while some were just done to make the code work. Certainly, I fell prey to the problem of scope creep, but I managed to get the code done the way I wanted it to be :)

Listing all of the changes here:

	1. Changed the python cryptographic library used from PKCS1_V1_15 to pkcs1_15
 
	2. Added features of Auto signing transaction on creation (no need to call the funciton separately)
 
	3. Included transaction signature within the transaction information
 
	4. Included feature for validation of transactions
 
	5. Added a property to the block class that would return the block header of a given block instance
 
	6. Added property to the Block class that would return all transactions contained within the given block instance.
 
	7. Integrated transaction searching as well as verification/validation inside the Block class itself (which means these tasks would be done under a single function of the block instance itself)
 
	8. Improved the logic of mining function used
 
	9. Implemented a makeshift Merkle Root 
 
 		[Merkle Root is the root of a tree hash structure, in which every transaction's hash is included and arranged in a tree structure. In the given code, All transactions have been appended into a single string and then their hash is calculated, simply for demonstration purposes. Certainly, the correct implementation could be made in a future endeavor.]
   
	10. Added mining as a method/function of the Block object  (so, again, the Block instance itself has the mining function which will calculate the nonce, hash and so on)
 
	11. Added 'Nonce' property to the blocks, (where nonce would be the current unix timestamp), while keeping functionality simple 
 
		(I am aware of the security implications that such implementation puts forward, however, this project is for demonstration purposes only, and the problem could be solved certainly, in any future implementation)
  
	12. Added functionality of Genesis block (as per tutorial) and modified it to suit the new code
 

Feel free to communicate for updates. Although I don't think I would be working to improve this specific blockchain, I do intend to take out parts of it's functionality if need be in the future. If I have missed out on any comments or if any code needs clarification, you can reach out to me for that as well :)
That's all! Good Day.
