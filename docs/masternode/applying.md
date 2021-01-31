Once your full node is up and running, you need to apply to make it eligible as a masternode.

Masternodes will receive a significant amount of block rewards, which likely exceeds the cost for running the infrastructure.
However, masternode candidates need to invest in Tao by depositing at least 100,000 Tao, and stake them for a long term.
Furthermore, after the initial deposit to become a candidate, if he doesn't make it to the top 150 most voted candidates, he will not be promoted as masternode and thus receive no rewards.
Therefore, candidates have an incentive to do as much as they can such as signalling their capability to support Tao to get into top 150 most voted candidates.

## Requirements
To have a masternode candidate, the following requirements must be satisfied:

- The token holder has an up and running node -- see our [documentation](https://docs.tao.network/masternode/taomn/).

- The token holder must hold a minimum required amount of tokens (100,000 TAO).
These 100,0000 TAO are deposited to the Voting Smart Contract.

- Must be one of the 150 most voted masternode candidates in the system.
The voting by token holders is credited through a Voting DApp that allows token holders to send TAO through the smart contract mechanism.

## Applying to become a masternode
You can apply by going on [Shifu](https://shifu.tao.network).
Connect the wallet that contains the funds you want to deposit.

!!! warning
    The wallet who makes the initial deposit will be the one receiving block rewards.

On the top right corner, click on "Become a Candidate".

Enter the amount of TAO you want to deposit (minimum 100,000).

Enter your coinbase address. This is the address of the account that your masternode is using.
If your are running your node with `taomn`, you can simply run `taomn inspect` to get it.

!!! note "Important note:"
	We advise for security measures to use a fresh new account for your masternode or 'coinbase address'.
	This is not the account that will receive the rewards.
	The rewards are sent to the account that will make the 100k TAO initial deposit.

Confirm with apply and proceed to make the payment.

Your full node will now be listed on Shifu.
People can view its details and vote for it.

A candidate becomes a masternode when it belongs to top 150 most voted candidates in each epoch.

!!! info
    An epoch is a period of 360 blocks (~ 30 minutes) starting from block #1

If your node is in the top 150 most voted candidates at the checkpoint between two epochs, it will be promoted as a masternode and will start producing blocks at the next epoch.

## Resigning your masternode
In case you want to stop your node, you need to resign it from the governance first in order to retrieve your locked funds.
Access Shifu, go to your candidate detail page, and click the `Resign` button.
Your funds will be available to withdraw 75 days after the resignation.

After resigning successfully, you can stop your node. If you ran it with `taomn`, simply run:
```
taomn remove
```

At this point, your masternode is completely terminated.
