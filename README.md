# base46
Testing Smart Contract Deployment Speed on Base  Developers often choose Base for its short confirmation times.
Python Example: deployment time benchmark
import time
from web3 import Web3

w3 = Web3(Web3.HTTPProvider("https://mainnet.base.org"))

start = time.time()
tx = w3.eth.get_block("latest")
end = time.time()

print("Response time:", end - start, "seconds")
Try same test on ETH and compare.
