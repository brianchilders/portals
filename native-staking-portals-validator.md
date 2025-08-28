# Native Staking - Portals Validator

## Background

In Solana, every validator operates with two key addresses, each serving a distinct role in the network.

#### Identity Account

* Name: Validator Identity
* Purpose: This is the validator’s public key — essentially their “main” account.
* Used for: Signing transactions, receiving rewards, and managing validator operations.
* Visibility: Often used to identify the validator in explorers and dashboards.

#### Vote Account

* Name: Validator Vote Account
* Purpose: This is the account that receives delegated stake and participates in consensus.
* Used for: Voting on blocks, earning staking rewards, and tracking validator performance.
* Visibility: This is the address you delegate to when staking SOL.

#### Relationship Between Them

* The vote account is controlled by the identity account.
* When you stake SOL, you delegate to the vote account, not the identity account.
* If you're manually staking via CLI or scripting validator interactions, always target the vote account for delegation.

## Staking on the Portals Validator

Using what we learned, the Portals Validator has two addresses:

Identity Account: prt1st4RSxAt32ams4zsXCe1kavzmKeoR7eh1sdYRXW

Voting Account: prt1s9dMM15LdsUX9HugajzqPB5WVN8a2mw3frAiCfj

You will always want to target the voting account for delegation.

This illustration is done using the Phantom wallet.  YMMV.

Open up the Phantom wallet and click on the Solana token

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

You will see options on how to use your SOL.  Click on the three dots (\*\*\*) / "More".

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Click on "Stake SOL"

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

Click on Native Staking

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Enter in the voting account address in the search window.  In this case, for the Portals validator, it is: prt1s9dMM15LdsUX9HugajzqPB5WVN8a2mw3frAiCfj

Then click on the Portals validator link

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Enter how much SOL you want to stake and click on the Stake button.

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

You are now staking natively with the Portals validator!
