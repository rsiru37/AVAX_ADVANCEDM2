# Happy HyperChain - Avalanche

This Project basically creates a Custom Hyper Chain and executes simple Actions that creates & Mints the assets to the receipitant's address, using HyperSDK Module by Avalanche

## Description

This Project is forked from tokenvm repository where we are would be using HyperSDK and making minor modifications to the files(constants.go & registry.go) and executing the respective actions of creating and minting the assets, after starting the node and build successful.

## Getting Started

### Installing

1. Inside the Project Directory, run go mod tidy to normalize the dependencies
2. Make sure Go is on your path, defined on your terminal, if not you can do so by running `export PATH=$PATH:$(go env GOPATH)/bin`
3. In First Terminal run `./scripts/run.sh`
4. In Second Terminal run `./scripts/build.sh`
5. Run `./build/token-cli key import demo.pk`
6. Run `./build/token-cli chain import-anr`
7. Now our project is ready and our HyperChain and the Avalanche Network are connected, Now we can execute any actions we like

### Executing program

1. Run `./build/token-cli action create-asset`
2. Set the Metadata for the asset and hit enter
3. We will be returned with an ID thats our asset ID
4. Run `./build/token-cli action mint-asset`
5. After running the above command it will ask us to enter the Asset ID, do paste the ID that we have generated in the create-asset step
6. Enter the recipient's address
7. Enter the Quantity to mint and hit Enter
8. You can verify the minting by executing `./build/token-cli key balance`

## Authors

Raj Siruvani - rajsiruvani@gmail.com
