# Healthcare Data NFT Vault

## Team Members:
| Name                          | CWID       | Email                             |
|-------------------------------|------------|-----------------------------------|
| Venkata Abhinav Karthik Pulikonda | 885210294 | abhinavpulikonda@csu.fullerton.edu |
| Manoj Gangavarapu             | 885164319  | manojgangavarapu@csu.fullerton.edu |
| Sai Satya Jagannadh Doddipatla| 885177436  | saijagannadh@csu.fullerton.edu     |
| Rakesh Puppala                | 885175919  | rakeshpuppala2591@csu.fullerton.edu |

---

## Project Description
The **Healthcare Data NFT Vault** leverages blockchain technology to securely tokenize sensitive healthcare data. The project enables users to encrypt and transform their healthcare data into Non-Fungible Tokens (NFTs), store the encrypted data on the InterPlanetary File System (IPFS), and manage access permissions using Ethereum smart contracts.

### Key Features:
- **NFT Minting**: Transform healthcare data into secure, encrypted NFTs.
- **Secure Storage**: Store encrypted data on IPFS, linking metadata to the IPFS hash.
- **Access Control**: Allow users to manage access by granting or revoking permissions for specific data.
- **Data Viewing**: Enable authorized users to decrypt and view healthcare data securely.

This project addresses the critical need for secure healthcare data sharing while ensuring privacy and compliance with regulations such as HIPAA.

---

## Project Overview
### Accomplishments:

1. **Smart Contract Development**:
   - Created core functionalities in Solidity for NFT minting, access granting, and revocation.
   - Integrated validations for token ownership and unique token IDs to enhance security.

2. **Frontend Development**:
   - Built a React-based interface for seamless user interaction.
   - Improved UI/UX with a simple, intuitive design.

3. **IPFS Integration**:
   - Integrated Pinata for storing encrypted healthcare data on IPFS.
   - Implemented encryption and decryption using CryptoJS to ensure data privacy.

4. **Access Control**:
   - Developed robust mechanisms for access control, enabling users to grant/revoke access to specific tokens.
   - Ensured only token owners can manage permissions through additional validations.

5. **Data Viewing**:
   - Implemented secure processes for authorized users to decrypt and view data.
   - Added detailed logging and error handling for a smooth user experience.

6. **Testing and Validation**:
   - Conducted comprehensive testing for all features, including minting, access granting, and decryption.
   - Fixed bugs related to user validation and decryption processes.

7. **Holesky Testnet Integration**:
   - Utilized the Holesky Testnet for testing in a blockchain environment, providing a better alternative to localhost.

---

## Features

1. **Patient Data Minting**:
   - Tokenize patient data fields such as Token ID, Data Type, Images, Date of Record Entry, and Healthcare Data Description.

   *(Insert photo here)*

2. **Access Control**:
   - Enable doctors to access patient data using randomized decryption keys (Token ID, Doctor Account Address, Decryption Key).

   *(Insert photo here)*

3. **Data Viewing**:
   - Allow doctors to securely view patient data (Token ID and Doctor Account Address).

   *(Insert photo here)*

4. **Other Features**:
   - Enhanced encryption and user authentication mechanisms.

---

## Setup and Run the Project

### Steps:

1. **Set Up Ganache Workspace**:
   - Open Ganache and create a new workspace.
   - Add the `truffle-config.js` file from the project.
   - Start the workspace.
   *(Insert photo here)*

2. **Install Dependencies**:
   ```bash
   npm install
   npm install -g truffle
   ```

3. **Note Down Contract Address**:
   - Open Ganache, navigate to the project, find the contract address, and update it in `client/src/app.js`.

4. **Configure Pinata**:
   - Update API credentials:
     ```javascript
     const PINATA_API_KEY = "XXXXXXXX";
     const PINATA_API_SECRET = "XXXXXXXXXXXXXXXXXXXXXX";
     ```

5. **Run the Frontend**:
   ```bash
   cd client
   npm start
   ```

6. **MetaMask Setup**:
   - Create a local network with the following settings:
     - **Network Name**: Localhost 8545
     - **RPC URL**: http://127.0.0.1:7545
     - **Chain ID**: 1337
     - **Currency Symbol**: ETH
     - **Block Explorer URL**: Leave blank.

   - Import accounts using private keys from Ganache:
     - Copy private keys from Ganache (Accounts > Address > Private Key).
     - Import them into MetaMask to create accounts for the patient and doctor.

7. **Mint Patient Data and Grant Access**:
   - Use the imported accounts in MetaMask for minting and access control.

---

## Issues, Challenges, and Questions

- **Encryption and Decryption**:
  - Debugged issues with malformed decryption keys by improving validation and logging mechanisms.

- **Smart Contract Integration**:
  - Resolved challenges in granting access by adding proper validations in both smart contracts and the frontend.

- **UI Enhancements**:
  - Iterated designs to create a more user-friendly and responsive interface.

- **Blockchain Gas Fees**:
  - Considered potential deployment issues related to high gas fees.

---

## Live Demo
*(Insert live demo video link here)*
