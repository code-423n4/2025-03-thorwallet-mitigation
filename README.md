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
[ ⭐️ SPONSORS ADD A LINK TO THE BRANCH IN YOUR REPO CONTAINING ALL PRS ]

### Mitigation of High & Medium Severity Issues
[ ⭐️ SPONSORS ADD ALL RELEVANT PRs TO THE TABLE BELOW:]

Wherever possible, mitigations should be provided in separate pull requests, one per issue. If that is not possible (e.g. because several audit findings stem from the same core problem), then please link the PR to all relevant issues in your findings repo. 

| URL | Mitigation of | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/your-repo/sample-contracts/pull/XXX | H-01 | This mitigation does XYZ | 

### Additional scope to be reviewed
[ ⭐️ CAS PLEASE REMOVE THIS SECTION IF THE SPONSOR IS ONLY MITIGATING HMS]

[ ⭐️ SPONSORS ADD ALL RELEVANT PRs TO THE TABLE BELOW:]

These are additional changes that will be in scope.

| URL | Reference ID | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/your-repo/sample-contracts/pull/XXX | ADD-01 | This mitigation does XYZ | 

## Out of Scope

Please list any High and Medium issues that were judged as valid but you have chosen not to fix.
