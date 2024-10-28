### Decentralized Delivery Platform

#### Overview
This platform is a decentralized delivery solution, using blockchain technology to provide a secure, transparent, and efficient way to manage package deliveries. By leveraging smart contracts and The Graph protocol, it ensures that all transactions are trustworthy and data retrieval is efficient. Users can manage their own deliveries, while delivery agents have the tools to view and fulfill orders, all in a secure and user-owned environment.

#### Key Features

1. **Wallet Integration**: Users can connect their digital wallets (e.g., MetaMask) to the platform for blockchain transactions.
2. **Role Selection**: Users have the option to choose roles within the app, acting as either a Sender/Recipient or as Delivery Personnel.
3. **Package Management**: Users can create, track, and manage package deliveries securely through smart contracts.
4. **Real-Time Data**: The platform utilizes The Graph for fast access to data such as delivery history, ratings, and completion rates.

#### Technologies Used

- **Arbitrum**: Manages on-chain delivery transactions with smart contracts.
- **The Graph**: Enables fast and efficient data retrieval from the blockchain.
- **Apollo Client**: Manages GraphQL queries between the frontend and The Graph.
- **Next.js**: Framework for building the responsive and dynamic user interface.
- **Web3.js**: Facilitates Ethereum blockchain interactions.

#### How It Works

##### Smart Contracts for Delivery and Ratings

The platform’s functionality is driven by smart contracts, which handle deliveries and ratings. Key operations include:

1. **Order Creation**: Each order includes important details (e.g., sender, recipient, delivery instructions), and each transaction is securely logged on the blockchain.
2. **Delivery Management**: The smart contract tracks package status updates, such as when a package is picked up or delivered, visible to all relevant parties.
3. **Delivery Confirmation and Payment**: When the recipient confirms delivery, the smart contract automatically transfers payment to the delivery agent.
4. **Rating System**: After each delivery, users can rate their experience, helping to ensure accountability and reliability among delivery agents.

##### Real-Time Data Retrieval Using The Graph

The platform uses The Graph protocol to create a subgraph that indexes all key events from the smart contracts, allowing real-time data access. Here’s how The Graph enhances data efficiency:

- **Subgraph Indexing**: Events like package creation, updates, and delivery confirmations are indexed for quick data access.
- **GraphQL Integration**: The frontend uses GraphQL to fetch data from The Graph efficiently:

    - **Get Packages**: Retrieves all packages associated with a specific user’s role and address.
    - **Get Ratings**: Shows user feedback on completed deliveries.
    - **Get Completion Rate**: Provides delivery completion statistics for individual delivery agents.

#### Installation

To set up and run the application, clone the repository and install dependencies:

```bash
git clone https://github.com/Okelo123/JUMTRACK.git
cd JUMTRACK
npm install
```

Then, start the development server:

```bash
npm run dev
```

#### Contributing

To contribute, fork the repository, make your changes, and submit a pull request for review.
