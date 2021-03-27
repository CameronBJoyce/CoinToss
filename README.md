# CoinToss “TOSS” 
ERC-20 Token built in Solidity


<img src="https://user-images.githubusercontent.com/61301130/112721546-c68bd680-8eda-11eb-9474-3cc10b32571e.gif" width="260" height="230"/>


1. Each time a coin is moved it is **flipped**
2. Each time a coin is held for one week, it is **flipped**
3. If a coin lands **on heads, value is doubled**, if it lands **on tails, coin value moves to 0.**
4. Tails coins can either be held for 1 week to be reflipped or they can be **moved** a **maximum of once per day**.
5. If head coins land **on heads twice in a row**, this coin can be used to** flip 2 additional tails** to heads as well. 
6. If tail coins land on tails twice in a row, the coin is **burned** from the network.

**Technical Specifications:**

**TOSS** is an ERC-20 Token built using the Solidity language. 

TOSS token functionality mirrors other popular tokens, but has an **_active update_** feature that automatically executes real-time, smart contracts to provide the core functionality of TOSS.

Key differences between TOSS and other tokens is the restriction of  movement and the active update feature.. If the coin can only be moved once a day, then this promotes the active maintenance of your portfolio and the development of trading bots to manage your portfolio across a longer period of time.

The protocol functionality of this coin focuses on ensuring:
*   **Control of the initial number of coins and issues;**
    *   Each user begins with 250 coins and then can trade or maintain their portfolio how they see fit. Theoretical buy-in cost would be $5 and then you get 250 coins and access to the trading network.
*   **Assignment of the initial quantity to the company's address and to the ICO members.**
    *   The owner will only receive 5% of initial tokens, the rest will be held in a central trust where owners who pay the entry fee can earn more tokens by landing on heads.
*   **Sending assets to investors, recording the balance.**
    *   TOSS users pay to purchase tokens from other users. The central trust is only used for distributing earnings, not as a central marketplace for purchases.
*   **Distribution of coins among users for transactions, verification of their movement.**
    *   Verification of movement will happen as 1 of two ways. Users can opt to pay a small slice of the earnings from landing on heads, or they can slightly increase (~2%) the probability of them landing on tails.
*   **Checking the remaining balance.**
    *   Standard token functionality as the central trust and users who pay a small slice of the earnings will be validators for ensuring current balances are correct.
*   **Control the adequacy of the currency at the address for transmission.**
    *   The _active update _functionality of the token will provide a constant stream of data as to the condition and current state of each TOSS token.

**Smart contracts have three classic functions:**
1. Conducts transactions, transfers tokens.** 2**. Confirms cost.  **3.** Tracks account balance.

**However, TOSS Smart Contracts have several functions built on top of this for each token:**
1. Tracks _Transfer_Time, Resting_Time, STATE (Heads or Tails),  PREVIOUS STATE_, _Daily # of transfers _(Heads = 10 limit, Tails = 1 limit).
2. Executes different operations on tokens/transactions depending on the different combination of information above.

**Composition:**

**Total # of Tokens**: 250,000,000 | **ICO cut**: 12.5 Million | **Trust**: 237,500,000 | **Buy In:** 250 Tokens

**Example:**

HEAD → HEAD = 1 additional, flipped coin inserted in your account from the central trust 

HEAD → TAIL = Coin value reduced to 0x (dud state)

TAIL → HEAD = Coin value returned to 1x (resting state)

TAIL → TAIL  = Coin removed from network (burned, deflationary)

