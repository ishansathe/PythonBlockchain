# PythonBlockchain
 Demonstrating the working and structure of blockchain with python programming language

The base code was referred from the following tutorial:
https://www.tutorialspoint.com/python_blockchain/index.htm


Many changes were made to the code, some were to improve the code, some were to satisify my interest, while some were just done to make the code work. Certainly, I fell prey to the problem of scope creep, but I managed to get the code done the way I wanted it to be :)

Listing all of the changes here:
	1. Changed the cryptographic library used from PKCS1_V1_15 to pkcs1_15
	2. Auto signing transaction on creation (no need to call the funciton separately)
	3. Included transaction signature within the transaction information
	4. Included validation of transactions
	5. Added a property to the block to return block header
	6. Added property ot block to return the included transactions
	7. Integrated transaction searching and verification/validation inside the block class
	8. Improved the logic of mining function used
	9. Implemented a makeshift Merkle Root (simplistic functionality to demonstrate use)
	10. Added mining as a method/function of the Block object
	11. Added 'Nonce' property to the blocks, (where nonce would be the unix timestamp), while keeping functionality simple 
		(Ofcourse, I am aware of the security problems that this may result in, but this is a demo blockchain so changes and precautions can be made and taken surely.)
	12. Added functionality of Genesis block (as per tutorial) and modified it to suit the new code
	13. Set the Max transaction count in block to 3

Feel free to communicate for updates. Although I don't think I would be working to improve this specific blockchain, I do intend to take out parts of it's functionality if need be in the future. If I have missed out on any comments or if any code needs clarification, you can reach out to me for that as well :)
That's all! Good Day.
