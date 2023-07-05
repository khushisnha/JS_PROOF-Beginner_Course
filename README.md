# JS_PROOF-Beginner_Course
It includes the Final Project explanation assigned at the end of the course by Metacrafters.

EXPLANATION OF CODE:

This code defines an array called myNFTs and several functions to interact with it. Going  through the code step by step:

1. The array myNFTs is initialized as an empty array. This array will store objects representing NFTs (Non-Fungible Tokens). //let myNFTs = [];

2. function mintNFT (name, age, profession, salary) {
    let nft = 
    {
        name: name,
        age: age,
        profession: profession,
        salary: salary
    };
    myNFTs.push(nft);
}

The function mintNFT is defined with four parameters: name, age, profession, and salary. This function creates a new object representing an NFT using the provided parameters and adds it to the myNFTs array using the push method.

push() method: this method is used to ass new items at the end of the array.

3. function listNFTs () {
    for(let i=0; i<myNFTs.length; i++)
    {
        let nft = myNFTs[i];
        console.log("\nID:"+(i+1));
        console.log("Name: " + nft.name);
        console.log("Age: " + nft.age);
        console.log("Profession:" + nft.profession);
        console.log("Salary: " + nft.salary);
        console.log("---------------------------------\n");
    }

}

The function listNFTs is defined without any parameters. It uses a for loop to iterate over each NFT object in the myNFTs array. Inside the loop, it prints the metadata of each NFT, including its ID (the index + 1), name, age, profession, salary, and a separator line.

4. function getTotalSupply() {
    return myNFTs.length;
}

The function getTotalSupply is defined without any parameters. It returns the length of the myNFTs array, which represents the total number of NFTs that have been minted.

5. mintNFT("khushi", "20", "Software Engineer", "50,000");
mintNFT("harshit", "20", "Blockchain developer", "80,000");
mintNFT("Bob", "29", "App Developer", "1,00,000");

The code calls the mintNFT function three times, passing different values for each NFT's metadata.

6. After minting the NFTs, the listNFTs function is called, which displays the metadata of each NFT in the console. //listNFTs();

7. Finally, the getTotalSupply function is called, and the returned value (the total number of minted NFTs) is concatenated with the string "Total Supply: " and printed to the console.
//console.log("Total Supply: " + getTotalSupply());

Thank you!
