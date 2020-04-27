# USDG Backed by United States Dollar

> Fiat backed Stablecoin Developed by Greyzdorf BTR LLC

<img src="https://www.greyzdorf.io/images/svg/usdg.svg" style="margin-left:20px" width="220" height="220" />

> [More Information](https://exchange.greyzdorf.io/usdg)

This repo consists of the smart contract for the USDG (Greyzdorf Dollar) issued by Greyzdorf BTR LLC on 27-04-2020, backed by Fiat USD kept in custody at Prime Trust.

### Specification of the Property & Digital Share (APR) :

- Written in : Solidity v6.0.3 (Latest by this time)<br />
- Blockchain : Ethereum<br />
- Backed By : Fiat<br />
- Ticker : USDG<br />
- TotalSupply : Variable Supply<br />
- Decimal : 2<br />
- Burning : available<br />
- Minting : available<br />
- Freeze : available<br />
- Type of Asset : Fiat Backed Stablecoin<br />
- New Contract Address : 0x9De152C32d820EB2E1Df392854d4dF2f4F305530


### Features of Smart Contract :

1. Minting & Burning to ensure that it stays intact with lending amount
1. Freeze & Whitelisting features to prevent AML
1. Exclusive password protected functions

### SafeMath Function:
```solidity
contract SafeMath {
    
  function safeMul(uint256 a, uint256 b) pure internal returns (uint256) {
    uint256 c = a * b;
    assert(a == 0 || c / a == b);
    return c;
  }

  function safeDiv(uint256 a, uint256 b) pure internal returns (uint256) {
    assert(b > 0);
    uint256 c = a / b;
    assert(a == b * c + a % b);
    return c;
  }

  function safeSub(uint256 a, uint256 b) pure internal returns (uint256) {
    assert(b <= a);
    return a - b;
  }

  function safeAdd(uint256 a, uint256 b) pure internal returns (uint256) {
    uint256 c = a + b;
    assert(c>=a && c>=b);
    return c;
  }

}
```

### Contributors
Developed by Greyzdorf BTR LLC Technical Team on 28-02-2020
