Stack Escrow
Stack Escrow is a decentralized escrow protocol built on the Stacks blockchain using Clarity.
It ensures secure and transparent STX transactions between two parties by locking funds until conditions are met or a third-party arbiter intervenes.

Features
Lock STX safely until trade conditions are met
Release funds manually or automatically
Built-in time-based refund
Optional dispute resolution through arbiter
Transparent event logging

Technical Overview
Language: Clarity
Core Functions:
create-escrow → Initialize and fund an escrow
release-funds → Transfer locked STX to seller
refund-buyer → Return funds if trade fails or expires
resolve-dispute → Arbiter resolves dispute
get-escrow → View escrow details
Stored Data:
Buyer, Seller, Arbiter
Amount (uSTX)
Deadline (block height)
Status (pending, released, refunded)

Installation & Usage
Clone the repository:
git clone https://github.com/your-repo/stack-escrow.git
cd stack-escrow
Deploy using Clarinet:
clarinet contract deploy stack-escrow
Run tests:
clarinet test
