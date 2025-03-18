# THORWallet Mitigation Review
- Total Prize Pool: $3,000 in USDC
  - Warden awards: $2,000 in USDC
  - Judge awards: $750 in USDC
  - Scout awards: $250 in USDC
- [Warden guidelines for C4 mitigation reviews](https://code4rena.notion.site/Guidelines-for-C4-mitigation-reviews-ed10fc5cfbf640bd8dcec66f38b343c4)
- Starts March 18, 2025 20:00 UTC 
- Ends March 25, 2025 20:00 UTC 

## Important note 

Each warden must submit a mitigation review for *every* individual PR listed in the `Scope` section below. **Incomplete mitigation reviews will not be eligible for awards.**

## Findings being mitigated

Mitigations of all High and Medium issues will be considered in-scope and listed here.

- [H-01: The user can send tokens to any address by using two bridge transfers, even when transfers are restricted.](https://code4rena.com/evaluate/2025-02-thorwallet/findings/S-391)
- [H-02: MergeTgt has no handling if TGT_TO_EXCHANGE is exceeded during the exchange period](https://code4rena.com/evaluate/2025-02-thorwallet/findings/S-171)
- [M-01: Improper Transfer Restrictions on Non-Bridged Tokens Due to Boolean Bridged Token Tracking, Allowing a DoS Attack Vector](https://code4rena.com/evaluate/2025-02-thorwallet/findings/S-125)

[ ⭐️ SPONSORS ADD INFO HERE ]

## Overview of changes [optional]

Please provide context about the mitigations that were applied if applicable and identify any areas of specific concern. 

## Scope

### Branch
https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-1
https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-2
https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-3
https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-4

### Mitigation of High & Medium Severity Issues
Wherever possible, mitigations should be provided in separate pull requests, one per issue. If that is not possible (e.g. because several audit findings stem from the same core problem), then please link the PR to all relevant issues in your findings repo. 

| URL | Mitigation of | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/4 | H-01 | Only allow bridging to the sender's own address | (F-9)
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/2 | H-02 | Fix issue when depositing more TGT and specified in the contract | (F-6)


### Additional scope to be reviewed
These are additional changes that will be in scope.

| URL | Reference ID | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/1 | ADD-01 | Fix issue claiming TITN on day 360 | (F-3)
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/3 | ADD-02 | This mitigation does XYZ | (F-4) 


## Out of Scope

Please list any High and Medium issues that were judged as valid but you have chosen not to fix.
[M-01: Improper Transfer Restrictions on Non-Bridged Tokens Due to Boolean Bridged Token Tracking, Allowing a DoS Attack Vector](https://code4rena.com/evaluate/2025-02-thorwallet/findings/S-125)
