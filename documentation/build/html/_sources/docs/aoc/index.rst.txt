Application of Concepts
=======================

.. image:: images/blankspace.png


Stakeholders
++++++++++++

.. image:: images/stackHolders.png


.. image:: images/blankspace.png

Tentative Smart Contracts
+++++++++++++++++++++++++

+--------------------------+-------------------------------------+
| Stakeholders             | Transactions                        |
+--------------------------+-------------------------------------+
| Tender Creator           | createNewTender()                   |
|                          +-------------------------------------+
|                          | uploadTenderInfoDocuments()         |
|                          +-------------------------------------+
|                          | sendTenderForApproval()             |
|                          +-------------------------------------+
|                          | addCorrigendum()                    |
|                          +-------------------------------------+
|                          | republishTender()                   |
|                          +-------------------------------------+
|                          | submitTenderTemplates()             |
+--------------------------+-------------------------------------+
| Tender Manager           | approveTender()                     |
|                          +-------------------------------------+
|                          | publishTender()                     |
|                          +-------------------------------------+
|                          | setTenderOpeningDate()              |
|                          +-------------------------------------+
|                          | setTenderClosingDate()              |
|                          +-------------------------------------+
|                          | publishInvitationForBids()          |
|                          +-------------------------------------+
|                          | viewSubmissions()                   |
+--------------------------+-------------------------------------+
| Bidder                   | uploadDigitalSignatureCertificate() |
|                          +-------------------------------------+
|                          | submitEarnestMoneyDeposit()         |
|                          +-------------------------------------+
|                          | uploadBidTechnicalDocuments()       |
|                          +-------------------------------------+
|                          | uploadBidFinancialDocuments()       |
|                          +-------------------------------------+
|                          | viewResult()                        |
|                          +-------------------------------------+
|                          | withdrawBid()                       |
|                          +-------------------------------------+
|                          | resubmitBid()                       |
+--------------------------+-------------------------------------+
| Bid Evaluation Committee | evaluateBidFinancialDocument()      |
|                          +-------------------------------------+
|                          | evaluateTechnicalDocument()         |
|                          +-------------------------------------+
|                          | assignExperts()                     |
|                          +-------------------------------------+
|                          | approveBestBid()                    |
|                          +-------------------------------------+
|                          | rejectBid()                         |
+--------------------------+-------------------------------------+
| Chief Vigilance Officer  | reviewTenderActivity()              |
|                          +-------------------------------------+
|                          | authoriseTender()                   |
|                          +-------------------------------------+
|                          | provideUniqueIdentificationNumber() |
|                          +-------------------------------------+
|                          | validateAwardContract()             |
|                          +-------------------------------------+
|                          | submitFinalBidderApproval()         |
+--------------------------+-------------------------------------+
| Fulfilment Manager       | validateOrderDetails()              |
|                          +-------------------------------------+
|                          | submitPaymentInfo()                 |
|                          +-------------------------------------+
|                          | submitDispatchDate()                |
|                          +-------------------------------------+
|                          | submitQualityReport()               |
+--------------------------+-------------------------------------+

.. image:: images/blankspace.png

Usecases
++++++++

.. figure:: images/biddingUsecase.png
     :align: center

     Bid Evalution Usecase flow (One can open the image in new tab by right click for better view)


* The usecase of Bid Evaluation Committe  - in this scenario the committe receives the bid document which is highly confidential, thus members of the committe need to submit a non-disclosure agreement.This legal contract is generated via Accord project.
  The contract is submitted to the chaincode container which eventually runs on the ledger.The blockchain-based business network on the Hyperledger Fabric invokes Accord Project components to execute Smart Legal Contracts.
* Similarly, once winning bidder is shortlisted via evaluation the Award Contract can be generated by the Cicero and logical smart legal functionality can be added by Ergo.
  Eventually, chaincode will be triggered and transactions will be saved on the fabric ledger.
