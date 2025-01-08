# AgriSupplyChain Smart Contract

This is a smart contract for an Agricultural Supply Chain system implemented using Solidity on the Ethereum blockchain. It tracks the journey of a product from the harvest stage to the customer, including ownership transfers, product updates, retailer details, and customer reviews.

## Features

1. **Create Product**: Allows the creation of a new product with details such as name, image, location, and transport stage.
2. **Ownership Transfer**: Transfers product ownership along the supply chain, with automatic state transitions between Harvest, InProduction, Retailer, and Customer stages.
3. **Update Chain**: Updates product details during the production stage.
4. **Retailer Details**: Allows retailers to record sales, stock received, price, and location details.
5. **Customer Review**: Lets customers review products after purchase, including quality, rating, description, and price feedback.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/agri-supply-chain.git
Install necessary dependencies:

bash
Copy code
npm install
Deploy the contract using Remix IDE or any other Ethereum development tool.

Contract Structure
Structs
Product: Holds details of the product, including its ID, name, owner(s), current state, transport stage, and financial information.
RetailerStage: Holds details about the product's stage in the retail process, such as sales, stock received, price, and location.
Review: Stores customer reviews, including quality, rating, description, and price review.
Enums
State: Enum representing the various stages a product goes through in the supply chain: Harvest, InProduction, Retailer, Customer.
Functions
CreateProduct: Creates a new product with details such as name, image, price, and transport stage.

TransferOwnerShip: Transfers ownership of the product to a new owner and updates its state.

UpdateChain: Updates the product details during the production stage.

RetialerDetails: Allows retailers to add their product-related details, such as sales and stock received.

CustomerReview: Enables customers to provide reviews on products once they have received them.

Deployment
To deploy this contract, you can use Remix IDE or deploy it through a Truffle or Hardhat project. Here is an example using Remix IDE:

Go to Remix IDE.
Copy and paste the Solidity contract into a new file.
Compile the contract.
Deploy the contract on the Ethereum test network or mainnet.
Usage
Once deployed, the contract can be interacted with by calling its public functions to create products, transfer ownership, update details, and collect reviews.

For example:

Create Product: Call the CreateProduct function to add a new product.
Transfer Ownership: Use TransferOwnerShip to transfer the product to the next stage.
Update Product: Update product details during the production stage using UpdateChain.
Retailer Details: Add retailer details using RetialerDetails.
Customer Review: Customers can add reviews using the CustomerReview function.
Contributing
If you'd like to contribute to this project, please fork the repository and submit a pull request. Ensure that your code follows the project's coding standards and passes all tests.
