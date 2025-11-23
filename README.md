@@ -149,7 +149,7 @@ USER_DECRYPTION_PRICE="1000000000000000000" # (uint256, 1 $ZAMA)
# For mocked test environments, the ZamaOFT address matches the deployer mocked contract's address, 
# while the FeesSenderToBurner address can be any address (no mocked contract needs to be deployed)
ZAMA_OFT_ADDRESS="0xc1D733116990ce3D9e54F9eCf48a1cdD441Af4f9" # ZamaOFT (address)
FEES_SENDER_TO_BURNER_ADDRESS="0xD75E59BF1DB5FB8bA7B3EEB75AcF1035f43ca3ad" # accounts[25] (address)
FEES_SENDER_TO_BURNER_ADDRESS="0x0000111122223333444455556666777788889999" # (address) (can be anything except address(0))

# Gateway contract address
# These addresses are required during the production deployment, at which point these environment 
@@ -163,3 +163,8 @@ PAUSER_SET_ADDRESS="0xC3F9e1D27Cd10402375B7CD237D57E0F4888C189" # PauserSet (add
# The first pauser's private key
# This is required for local tests and running the pausing task. It must correspond to one of the pauser's private key
PAUSER_PRIVATE_KEY="0x3588ffb4f4d9bea785a012b895543fe68f2d580a9d449decc91a25878064079a" # accounts[23], private key (bytes32)

# The private key of the account that sends request transactions (input verification, decryption) to the gateway (the relayer)
# This is only meant for local tests for mocked tokens funding and approval
# It must be the first account as this is the account used for transactions by default
TX_SENDER_PRIVATE_KEY="0x55c7e64a1e153d667b2ce7489b62e0c6d5716fcb016ab6dd324decccf4d2cb2f" # accounts[25], private key (bytes32)
