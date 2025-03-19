# THORWallet Mitigation Review
- Total Prize Pool: $3,000 in USDC
  - Warden awards: $2,000 in USDC
  - Judge awards: $750 in USDC
  - Scout awards: $250 in USDC
- [Warden guidelines for C4 mitigation reviews](https://code4rena.notion.site/Guidelines-for-C4-mitigation-reviews-ed10fc5cfbf640bd8dcec66f38b343c4)
- Starts March 20, 2025 20:00 UTC 
- Ends March 25, 2025 20:00 UTC 

## Important note 

Each warden must submit a mitigation review for *every* individual PR listed in the `Scope` section below. **Incomplete mitigation reviews will not be eligible for awards.**

## Findings being mitigated

Mitigations of all High and Medium issues will be considered in-scope and listed here.

- [F-9: The user can send tokens to any address by using two bridge transfers, even when transfers are restricted.](https://code4rena.com/evaluate/2025-02-thorwallet/findings/F-9)
- [F-6 MergeTgt has no handling if TGT_TO_EXCHANGE is exceeded during the exchange period](https://code4rena.com/evaluate/2025-02-thorwallet/findings/F-6)

Mitigations of these additional issues will also be considered in-scope:
- [F-3: User funds can get locked due to > instead of >= for Merge end time](https://code4rena.com/evaluate/2025-02-thorwallet/findings/F-3)
- [F-4: `TITN` tokens transferred to the `LayerZero` endpoint address will be lost](https://code4rena.com/evaluate/2025-02-thorwallet/findings/F-4)


[ ⭐️ SPONSORS ADD INFO HERE ]

## Overview of changes [optional]

Please provide context about the mitigations that were applied if applicable and identify any areas of specific concern. 

## Scope

### Branch
- https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-1
- https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-2
- https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-3
- https://github.com/THORWallet/TGT-TITN-merge-contracts/tree/audit-4

### Mitigation of High & Medium Severity Issues

| URL | Mitigation of | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/4 | F-9 | Only allow bridging to the sender's own address |
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/2 | F-6 | Fix issue when depositing more TGT and specified in the contract |


### Additional scope to be reviewed
These are additional changes that will be in scope.

| URL | Reference ID | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/1 | F-3 | Fix issue claiming TITN on day 360 |
| https://github.com/THORWallet/TGT-TITN-merge-contracts/pull/3 | F-4 | This mitigation does XYZ |


## Out of Scope
- [F-7: Improper Transfer Restrictions on Non-Bridged Tokens Due to Boolean Bridged Token Tracking, Allowing a DoS Attack Vector](https://code4rena.com/evaluate/2025-02-thorwallet/findings/F-7)
