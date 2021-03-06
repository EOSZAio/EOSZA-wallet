# Flowchart

## JavaScript style

Our JavaScript is formatted in the [AirBnB JS style](https://github.com/airbnb/javascript).

## CSS style

Our CSS style is in [AirBnB CSS styleguide](https://github.com/airbnb/css).

## Application startup

The wallet application startup process is;
1. Language not set
* Select language
2. Splascscreen
* Update blockchain API access point list (ilitially hardcoded)
* Test access point using "get_info" RPC call, if failed try next API point
* Check language
3. Main
* no account set, add account. NB, it is not necessary for the user to add their "active" private key to add an account to the wallet. The private key is only required when the user attempts to do something that requires a signature. This allows the wallet to be used to watch accounts.
* Refresh all accounts using "get_account" RPC call

Process shown in flow diagram below.

### Application startup flow diagram

![App startup](https://github.com/EOSZAio/EOSZA-wallet/blob/master/documentation/startup.png "App startup")

Drawn using https://www.draw.io
