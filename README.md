Blockchain Terminal

An interactive, visual blockchain simulator built with vanilla JavaScript, HTML, and Tailwind CSS. This project provides a hands-on demonstration of the core concepts of blockchain technology, all wrapped in a retro terminal-style interface.
✨ Features
 * Interactive Blockchain: Create a blockchain from scratch right in your browser.
 * Adjustable Difficulty: Set the mining difficulty (the number of leading zeros required for a valid hash) to see how it impacts mining time.
 * Transaction Creation: Add transactions to a "Memory Pool" before they are mined.
 * Visual Mining Process: Watch in real-time as the simulator performs "Proof-of-Work," iterating through nonces to find a valid block hash.
 * Chain Visualization: See the entire blockchain, with each block clearly displaying its index, timestamp, transactions, nonce, hash, and the previous block's hash.
 * Immutability Demonstration: Use the "Tamper" function to alter data in a previous block and instantly see how it breaks the cryptographic chain.
 * Built-in Explainers: Interactive SVG and code animations explain the fundamental concepts of how a blockchain works and the code behind it.
 * Retro Aesthetic: A fun, CRT-monitor-inspired theme built with custom CSS and the VT323 font.
🚀 How to Use
 * Initialize the Chain: Open the index.html file in your browser. First, select a mining difficulty from the dropdown menu and click Initialize Chain.
 * Create Transactions: Fill in the sender, receiver, and amount fields, then click Add to Pool. You can add multiple transactions.
 * Mine a Block: Once you have transactions in the Memory Pool, the Mine Block button will become active. Click it to start the mining process.
 * Observe the Process: A new "Mining..." block will appear at the top of the chain. You can see the nonce and hash changing rapidly as the simulator searches for a valid hash that meets the difficulty requirement.
 * See the Result: Once a valid hash is found, the block is "mined" and added to the top of the chain. The pending transactions are cleared from the Memory Pool.
 * Test Immutability: After mining at least one block, click the Tamper Chain button. This will change data in the first block, causing its hash to change and invalidating the entire chain from that point forward, visually demonstrated with red highlights and a "glitch" effect.
🛠️ Key Concepts Demonstrated
This simulator provides a tangible way to understand several core blockchain principles:
 * Blocks & Chain: The fundamental data structures where blocks of transactions are linked together chronologically.
 * Cryptographic Hashing: Each block has a unique hash (a digital fingerprint) generated from its contents. Any change to the block's data results in a completely different hash.
 * Proof-of-Work (Mining): The process of expending computational effort to solve a puzzle. In this case, finding a nonce that results in a block hash with a specific number of leading zeros.
 * Immutability: Because each block's hash is included in the next block, the chain is cryptographically secured. Altering a past block invalidates its hash, which breaks the link to the next block, and so on, making the ledger tamper-evident.
 * Memory Pool (Mempool): A waiting area for unconfirmed transactions before they are selected by a miner to be included in the next block.
 * Mining Rewards: A special transaction is automatically added to each new block, rewarding the miner for their work in securing the network.
💻 Technologies Used
 * HTML5: For the core structure of the application.
 * CSS3: For the retro styling, animations, and responsive layout.
 * Tailwind CSS: For utility-first CSS classes to accelerate development.
 * Vanilla JavaScript (ES6): For all of the application logic, including the blockchain classes, mining simulation, and DOM manipulation.
