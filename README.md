Project 1 Report - Gary Yip



PART 1

for k = 2, my xS value is 1611002137this_is_a_bitcoin_block_of_81736042. it's hash value is 00dac80d4b34a04c15f24009953c0f7077f4487ab0539d96483bb0fa6f47ff8a. time elapsed was 10 seconds and number of trials is 1000.

for k=3, my xS value is 797942122this_is_a_bitcoin_block_of_81736042. it's hash value is 0007b8050039c1d2cc43a61e019763734a374f46b091cf5f6633c630e7250b5a. Time elapsed was 10 seconds and number of trials is 10,000.

for k=4, my xS value is 904770128this_is_a_bitcoin_block_of_81736042. it's hash value is 0000023f79a6ab9442df7b3f63e92431750aa0edcb11eb009455c033717ba410. Time elapsed was 13 seconds and number of trials is 1,000,000. (this particular solution had 5 leading zeroes)

for k=5, my xS value is 1260639825this_is_a_bitcoin_block_of_81736042. it's hash value is 00000907b1d42cd52597bce8cf5ad35db23e545e6aff8ef54a7a497dca97d0b6. Time elapsed was 27 seconds and number of trials is 5,000,000.

for k=6, my xS value is 1365365373this_is_a_bitcoin_block_of_81736042. It's hash value was 000000d808d823eea01ba73bcbf62f3f2986ebd4e2f17e3bfa59fa235d549b0c. Time elapsed was 191 seconds and number of trials is 50,000,000.


PART 2

for k = 7, my xS value is 1624689558this_is_a_bitcoin_block_of_81736042. It's hash value is 0000000183278ce33193a42c665987a9a7afca83cd7df16428f57d8532c72bbc. Time elapsed was 1805s and number of trials is 500,000,000.

My cluster's configuration was set up just as instructed in the instructions. In terms of estimating the number of trials needed in order to find the nonce, I noticed that for ever increase in k, the number of trials would go up by roughly 10 times. (in some cases more, some cases less). As in part 1, I worked my way up somewhat following that pattern until in k=6 I was up to 50 million trials. I knew that this was not too many trials because the program told me that the count was only 1. I estimated 500 million trials, but initially tried out 100million. I did this because I noticed a massive, exponential increase in time elapsed for the program as I kept on adding an extra digit. Unfortunately, this yielded no results so I went a little bit higher and got it. 


PART 3
I believe this approach will be more efficient. This is because it is possible for the random number generator to repeat a chosen potential nonce again, which is an inefficiency. 