# Treasury

### Intro

While validators are often the only stakeholder natively incentivized in other blockchains, Edgeware proposes to use the block reward to incentivize all stakeholders. Block inflation will be allocated token towards an on-chain treasury,  which will be allocated by specific treasury proposals.

The treasury is funded through transaction fees, slashing, inefficiencies in the chain's staking set, and lost deposits. The funds held in the treasury can be spent by making a spending proposal that, if approved by the council, will enter a queue that is cleared every 24 days \(known as the budget period\). The treasury attempts to spend as many proposals in the queue as it can without running out of funds. If the treasury ends a budget period without spending all of its funds, it suffers a burn of a small percentage of its funds -- thereby causing deflationary pressure.

{% hint style="info" %}
 **Parameter Note:** Initially, the on-chain treasury will be funded by 50% of the block reward, with the other 50% going to validators. 
{% endhint %}

### Description of the Treasury

_From_ [_Web3 Foundation Research_](https://research.web3.foundation/en/latest/polkadot/Token%20Economics.html)\_\_

The system needs to continually raise funds, which we call the treasury. These funds are used to pay for developers that provide software updates, apply any changes decided by referenda, adjust parameters, and generally keep the system running smoothly.

Funds for treasury are raised in two ways:

1. by minting new tokens, leading to inflation, and
2. by channelling the tokens from transaction fees and slashings, which would otherwise be set for burning.

Notice that these methods to raise funds mimic the traditional ways that governments raise funds: by minting coins which leads to controlled inflation, and by collecting taxes and fines.

We could raise funds solely from minting new tokens, but we argue that it makes sense to redirect into treasure the tokens from tx fees and slashing that would otherwise be burned:

* By doing so we reduce the amount of actual stake burning, and this gives us better control over the inflation rate \(notice that stake burning leads to deflation, and we can’t control or predict the events that lead to burning\).
* Following an event that produced heavy stake slashing, governance might often want to reimburse the slashed stake partially, if there is a bug in the code or there are extenuating circumstances. Thus it makes sense to have the EDGs available in treasury, instead of burning and then minting.
* Suppose that there is a period in which there is an unusually high amount of stake burning, due to either misconducts or transaction fees. This fact is a symptom that there is something wrong with the system, that needs fixing. Hence, this will be precisely a period when we need to have more funds available in treasury to afford the development costs to fix the problem.

**Next**, read about proposing a Treasury Spend action.

