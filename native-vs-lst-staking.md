# Native vs LST Staking

Native staking and Liquid Staking Tokens (LSTs) both serve the same goal (earning rewards), but they behave very differently under the hood. Here are **five key differences** to keep in mind when staking natively vs using LSTs:

1\. **Epoch Timing & Activation Delay**

* **Native staking** follows Solana’s epoch cycle (\~2 days).
* When you delegate stake, it doesn’t become active immediately — it takes **one full epoch** to activate.
* Similarly, **unstaking** takes **one full epoch to deactivate**, and only then can you withdraw your SOL.
* **LSTs**, like mSOL, jitoSOL, or portalsSOL, skip this delay — you get a liquid token instantly and can trade or use it in DeFi right away.

2\. **Why Your Full Stake Balance Doesn’t Show**

* In **native staking**, only the **active portion** of your stake earns rewards and shows up in performance dashboards.
* If you just delegated or are in the process of unstaking, your SOL is in a **"activating" or "deactivating" state**, which doesn’t count toward rewards yet.
*   Phantom and CLI tools will show this split if you run:

    ```bash
    solana stake-account <STAKE_ACCOUNT_ADDRESS>
    ```

3\. **Deposits & Withdrawals Are Epoch-Locked**

* **Depositing SOL** into a stake account is instant, but **delegation** takes an epoch to activate.
* **Withdrawing SOL** requires:
  1. Deactivating the stake (1 epoch)
  2. Waiting for the epoch to end
  3. Then withdrawing the SOL
* With **LSTs**, you can sell or swap your token anytime, but you may face slippage or fees depending on liquidity.

4\. **Control vs Convenience**

* **Native staking** gives you full control over:
  * Which validator you support
  * Commission rates
  * Validator decentralization
* **LSTs** abstract this away — you stake into a pool, and the protocol spreads stake across validators. You lose direct control but gain flexibility.

5\. **Reward Visibility & Liquidity Risk**

* **Native staking rewards** accrue in your stake account and are visible epoch-by-epoch.
* **LSTs** often auto-compound rewards into the token’s value (e.g., portalsSOL increases in price over time).
* If you need to exit quickly, LSTs offer liquidity — but in volatile markets, you may get less than your original stake due to price fluctuations.

