# codealpha_tasks-
#codealpha # blackchain


###TASK-1
# Simple-storage-smart-contract.sol

# 🌟 SimpleStorage.sol: A Glimpse into Solidity Basics 🌟

This repository showcases `SimpleStorage`, a foundational Solidity smart contract designed to illustrate core concepts of blockchain development. Think of it as your friendly guide to understanding how data is stored, manipulated, and secured on the Ethereum blockchain.

---

## 💡 What's Inside?

The `SimpleStorage` contract is your digital vault for a single integer. Only the **owner** (the person who deploys it) can change this number, and every modification is meticulously logged through **events**, offering complete transparency.

---


## ✨ Key Features that Shine

* **`value` (The Heart of the Contract):** This private integer variable holds the one piece of data our contract manages. It's kept safe and sound within the contract's memory.
* **`owner` (The Gatekeeper):** An `address` type variable that permanently stores the identity of the contract's deployer. This address holds the keys to modify the `value`.
* **`constructor()` (The Grand Opening):** This special function runs only once, right when the contract comes to life on the blockchain. It sets the `owner` to whoever deploys the contract and initializes `value` to a clean `0`.
* **`onlyOwner()` (The Exclusive Club Bouncer):** A powerful **modifier** that acts as a guard. Any function adorned with `onlyOwner` can only be called by the contract's true `owner`. Try to sneak in without permission, and you'll be met with an "Access denied!" message!
* **`increment()` (Count Up!):** This function bumps the `value` up by one. But remember, `onlyOwner` can make this magic happen!
* **`decrement()` (Count Down!):** Just like `increment()`, this function nudges the `value` down by one, strictly for the `owner`'s use.
* **`getValue()` (Peeking Inside):** A handy function to simply view what the current `value` is. It's a `view` function, meaning it doesn't change anything and is completely free to call!
* **`ValueUpdated` (The Blockchain's Diary):** An **event** that acts like a public announcement board. Every time `value` changes, `ValueUpdated` broadcasts the `newValue`, what `action` was taken ("Incremented" or "Decremented"), and `updatedBy` who made the change. This makes every modification transparent and traceable on the blockchain.

---

## 🛠️ How It All Comes Together, Step by Step

### 1. The Blueprint (`pragma solidity ^0.8.0;`)
...............


###TASK-2 

