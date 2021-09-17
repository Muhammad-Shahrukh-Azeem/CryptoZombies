<h1>Bonus Task for CryptoZombies</h1>
Truffle project with unit testing and deployment to the local blockchain.
<h2>Ownable Contract</h2>
The Ownable contract has an owner address and provides essential authorization control
to the user.
It consists of many functions and a modifier that makes sure that the user has all the power.
<h2>SafeMath</h2>
This contract consists of many functions that allow us to safely perform mathematical calculations.
In case if an overflow occurs during an arithmetic operation, it will throw an error.
<h2>ZombieAttack<h/2>
This contract consists of functions that make the fun happen.
This contract contains functions that take a probability, and through that, it checks which player has won and then changes their scores accordingly.
<h2>ZombieFactory<h/2>
This contract contains functions that create random zombies for our game and updates them to the mapping.
One function here creates random DNA for zombies using hash encryption "Keccak."
It will also emit a event in its create zombie function
<h2>ZombieHelper<h/2>
This contract is responsible for handling all the changes which user wants to make to his zombie.
It contains functions that accept "ETHER" to allow users to level up (PAYABLE functions are used). Moreover, it can be used to view that how any zombie does a user have,     
<h2>ZombieFeeding<h/2>
This contract will restrict the user from attacking using a cooldown function.
Another function gives zombies the ability to feed by using a formula that gives zombies a new DNA and triggers a cooldown function.
A function here allows users to interact and feed on Zombie kitties.
<h2>ZombieOwnership<h/2>
This contract Handles all the Owner and keeps track of who has how many zombies and who is transferring to who.
It also contains some ERC721 function calls.
It allows users to transfer a zombie to different users and keep track of the Owner.
<h2>ERC721<h/2>
This contract Contains the standard implementation of ERC721 Functions and their events.
<h2>UnitTesting</h2>
Once we deploy our code to the blockchain, it will be there forever, so unit testing is important.
<li>The first test checks if the new zombie is created and assigned to the user.</li>
<li>The second test makes sure that only one zombie is created.</li>
<li>The third test makes the zombie transfer to the new user using one step scenario.</li>
<li>The fourth and fifth test makes the zombie transfer to the new user using a two-step scenario. This allows the user to approve a transaction so that anyone of the  two parties can cal tthe transaction later.</li>
<li>This last test makes sure that zombies can attack other zombies and cooldown function works.</li>
