# Counterparty Credit Risk Introduction

Counterparty credit risk (CCR) refers to the risk that a counterparty to a bilateral financial derivative contract may fail to fulfill its contractual obligation causing financial loss to the non-defaulting party. It will be incurred in the event of default by a counterparty.

If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default one. That is why counterparty credit risk sometimes is referred to as replacement risk.

Only over-the-counter (OTC) derivatives and financial security transactions (e.g., repo) are subject to counterparty risk. If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default one. That is why counterparty credit risk sometimes is referred as replacement risk. The replacement risk is the MTM value of a counterparty portfolio at the time of the counterparty default.

Counterparty credit risk measurement is credit exposure (CE). It is the cost of replacing or hedging a contract at the time of default. Other measures include Potential future exposure (PFE), Expected exposure (EE), Expected Positive Exposure (EPE), Effective expected exposure (EEE), Effective EPE, Exposure at default or EAD. This presentation is intended to answer several fundamental questions: what is CCR? How to measure CCR? What are the provisions governing counterparty risk?



	Counterparty Credit Risk Definition
	Counterparty credit risk refers to the risk that a counterparty to a bilateral financial derivative contract may fail to fulfill its contractual obligation causing financial loss to the non-defaulting party.
	The risk that a counterparty defaults prior to expiration of a contract.
	We define counterparty credit risk as the risk of loss that will be incurred in the event of default by a counterparty.
	Only over-the-counter (OTC) derivatives and financial security transactions (e.g., repo) are subject to counterparty risk.
	If one party of a contract defaults, the non-defaulting party will find a similar contract with another counterparty in the market to replace the default one. That is why counterparty credit risk sometimes is referred as replacement risk.
	The replacement risk is the MTM value of a counterparty portfolio at the time of the counterparty default.

	Counterparty credit risk measures
	Credit exposure (CE): the cost of replacing or hedging a contract at the time of default.
 
	Credit exposure is uncertain (stochastic) so that Monte Carlo simulation is needed
	Potential future exposure (PFE): credit exposure at specified quantile on a future date
	Expected exposure (EE): average (expected) credit exposure on a future target date.
	EPE (Expected Positive Exposure) – Weighted average of EE
	Effective expected exposure (EEE): max EE before time t
	Effective EPE: weighted average of Effective EE
	Exposure at default or EAD =  * EffectiveEPE; where   = 1.4
	Effective maturity M: some deals’ maturity over one year
 

 

	Close out
	If a contract value > 0 to the bank at the time of default, the bank
	Close out the position and receive nothing from the defaulting counterparty
	Enter a similar contract with another party and pay the contract value.
	The exposure is the replacement cost, i.e., the contract value
	If the contract value < 0 at the time of default, the bank
	Close out the position and paying contract value to the defaulting counterparty
	Enter a similar contract with another party and receives the contract value.
	The net loss is zero
	The credit exposure can be expressed as
E(t) = max(V(t), 0)

	Master Agreement
	Master agreement is a document agreed between two parties, which applies to all transactions between them.
	Close out and netting agreement is part of the Master Agreement.
	If two trades can be netted, the credit exposure is
E(t)=max(V_1 (t)+V_2 (t),0)
	If two trade cannot be netted (called non-netting), the credit exposure is
E(t)=max(V_1 (t),0)+max(V_2 (t),0)

	CSA Agreement
	CSA (or Margin Agreement or Collateral Agreement) is a legal document that regulates collateral posting.
	Trades under a CSA should be also under a netting agreement, but not vice verse.
	It defines a variety of terms related to collateral posting.
	Threshold
	Minimum transfer amount (MTA)
	Independent amount (or initial margin or haircut)
	Credit exposure after taking CSA into account
 

	Final Credit Exposure
	After taking master agreement and collateral into account, the final counterparty credit exposure equals
E_cpty (t)=∑_i▒〖E_NCi+∑_j▒〖E_Nj+∑_k▒E_NNk 〗〗
where 
E_NCi – the exposure for a trade with both CSA and netting agreement
E_NCi – the exposure for a trade with netting agreement but without CSA
E_NNk – the exposure for a non-netting trade

References:

https://finpricing.com/lib/IrSwap.html
