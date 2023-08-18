Project: Create a NFT Collection

The given code is written in JavaScript and involves creating and managing NFTs (Non-Fungible Tokens). NFTs are unique digital assets often used to represent ownership of digital or physical items in a blockchain-based environment. Let's break down the code step by step:

1. NFTs Array Initialization:
   
const NFTs = [];

This line initializes an empty array called NFTs to store the NFT objects that will be created using the 'mintNFT' function.

3. mintNFT Function:
   
function mintNFT(_name, _eyeColor, _shirtType, _shirtColor) {
    // Create an NFT object using the provided parameters
    const NFT = {
        "name": _name,
        "eyeColor": _eyeColor,
        "shirtType": _shirtType,
        "shirtColor": _shirtColor
    };

    // Add the NFT object to the NFTs array
    NFTs.push(NFT);

    // Print a message indicating the NFT has been minted
    console.log("Minted: " + _name);
}

The mintNFT function takes four parameters: _name, _eyeColor, _shirtType, and _shirtColor. It creates an NFT object using these parameters, adds it to the NFTs array, and logs a message indicating the successful minting of the NFT.

3. listNFTs Function:
   
function listNFTs() {
    for (let i = 0; i < NFTs.length; i++) {
        console.log("\nID: " + (i + 1));
        console.log("Name: " + NFTs[i].name);
        console.log("EyeColor: " + NFTs[i].eyeColor);
        console.log("ShirtType: " + NFTs[i].shirtType);
        console.log("ShirtColor: " + NFTs[i].shirtColor);
    }
}

The listNFTs function iterates through the NFTs array and prints out the metadata of each NFT object, including the ID (index + 1), name, eye color, shirt type, and shirt color.

4. getTotalSupply Function:

function getTotalSupply() {
    console.log("\n" + NFTs.length);
}

The getTotalSupply function simply prints the total number of NFTs minted, which is equal to the length of the NFTs array.

5. Function Calls:

mintNFT("Shubham", "Black", "Henley", "Beige");
mintNFT("Rishabh", "Brown", "Flannel", "Blue");
mintNFT("Sumoksh", "Brown", "Linen", "Black");
mintNFT("Anurag", "Black", "Polo", "Brown");
listNFTs();
getTotalSupply();

These lines call the mintNFT function four times with different parameters to mint four NFTs. Then, it calls the listNFTs function to display the metadata of all minted NFTs, and finally, it calls the getTotalSupply function to print the total number of minted NFTs.

Overall, this code simulates the creation, listing, and tracking of NFTs using JavaScript functions and an array to store the NFT objects' metadata.
