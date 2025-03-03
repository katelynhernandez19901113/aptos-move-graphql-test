
# aptos-move-graphql-test

## Leveraging ABIs: Prototype Demonstration with v1 Resource Representation

### Introduction

This project demonstrates the use of Aptos Move GraphQL API by leveraging ABI (Application Binary Interface) metadata to query smart contract resources efficiently. It serves as a prototype to explore how v1 resource representation can be used to interact with on-chain data in an optimized and structured manner.

### Features

-   Querying Move smart contract resources via GraphQL.
    
-   Utilizing ABI metadata to interpret resource structures.
    
-   Demonstrating efficient data retrieval with v1 resource representation.
    
-   Providing an example implementation for developers exploring Aptos Move and GraphQL integration.
    

### Prerequisites

To run this project, ensure you have the following installed:

-   Aptos CLI
    
-   [Node.js](https://nodejs.org/) (for running GraphQL queries)
    
-   [Docker](https://www.docker.com/) (optional for containerized execution)
    

### Installation

1.  Clone this repository:
    
    ```
    git clone https://github.com/katelynhernandez19901113/aptos-move-graphql-test.git
    cd aptos-move-graphql-test
    ```
    
2.  Install dependencies:
    
    ```
    npm install
    ```
    
3.  Start the GraphQL server:
    
    ```
    npm run start
    ```
    

### Usage

1.  Deploy a Move module on the Aptos testnet or devnet.
    
2.  Use the provided GraphQL queries to fetch resource data.
    
3.  Experiment with ABI-based interpretations of on-chain structures.
    

Example GraphQL query:

```
{
  getResource(accountAddress: "0x1", resourceType: "0x1::coin::CoinStore") {
    data {
      coin {
        value
      }
    }
  }
}
```

### Contribution

Contributions are welcome! Feel free to open issues and submit pull requests.

### License

This project is licensed under the MIT License.
