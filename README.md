# create-steel-app

## Dependencies

Make sure to have the following installed:

1. [Rust](https://www.rust-lang.org/tools/install)
2. [Foundry](https://book.getfoundry.sh/getting-started/installation)
3. [cargo-risczero](https://dev.risczero.com/api/zkvm/install)

## Usage

`curl -fsSL https://raw.githubusercontent.com/sashaaldrick/create-steel-app/refs/heads/main/create-steel-app -o create-steel-app.sh && bash create-steel-app.sh`

You can choose between two release versions: [1.0](https://github.com/risc0/risc0-ethereum/tree/release-1.0) and [1.1](https://github.com/risc0/risc0-ethereum/tree/release-1.1).

Once the script is finished running, you should:

```
cd PROJECT_NAME
cargo build
forge build
``` 

After this, you can export the necessary Bonsai environment variables:

```
export BONSAI_API_KEY="YOUR_API_KEY" 
export BONSAI_API_URL="BONSAI_URL" # provided with your api key
```

Note: To request an API key [complete the form here](https://bonsai.xyz/apply).

At this point, you will be able to test against a local deployment by running the provided bash script:

`./test-local-deployment.sh`


