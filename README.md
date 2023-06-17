// Step 1: Create a variable to hold the number of NFTs
let numberOfNFTs = 0;

// Step 2: Create an object inside the mintNFT function to hold the metadata for NFTs
function mintNFT(name, description, image) {
  const nft = {
    name: name,
    description: description,
    image: image
  };

  numberOfNFTs++; // Increment the number of NFTs

  // Store the NFT in a data structure of your choice, like an array or map
  // Here, we'll assume you store it in an array called nfts
  nfts.push(nft);
}

// Step 3: Print all NFTs' metadata using the listNFTs function
function listNFTs() {
  for (let i = 0; i < nfts.length; i++) {
    const nft = nfts[i];
    console.log("Name: " + nft.name);
    console.log("Description: " + nft.description);
    console.log("Image: " + nft.image);
    console.log("---------------------");
  }
}

// Step 4: Get the total supply of NFTs using the getTotalSupply function
function getTotalSupply() {
  return numberOfNFTs;
}

// Example usage:
const nfts = []; // Array to store NFTs

mintNFT("NFT 1", "Description 1", "image1.jpg");
mintNFT("NFT 2", "Description 2", "image2.jpg");
mintNFT("NFT 3", "Description 3", "image3.jpg");

listNFTs();
console.log("Total Supply: " + getTotalSupply());
