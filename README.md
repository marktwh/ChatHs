# ChatHs
## Introduction
This is a component that relays prompts to writers and holds payments in escrow until 3-500 word responses are submitted within a set timeframe. The payment is initially set at $20 and the response must be submitted within 24 hours for the writer to claim it. However, as additional prompts are added to the stack, the required payment doubles and the timeframe is extended by a further 24 hours each time. As each active 24 hours elapses, the required payment is reduced again accordingly.
## Writer
This is permissionless. The writer instantiates the component from the blueprint with a name and a 1-300 word 'bio' and awaits prompts. Instantiation returns a soulbound 'account' NFT required to respond to prompts.

Prompt NFTs are minted by the component upon receipt of the prompt and the appropriate payment. The writer can edit this NFT to add the necessary 3-500 word response within the required timeframe. This action requires the 'account' NFT. This action returns the payment minus a 10% commission.
## Prompter
The prompter sends a prompt of up to 100 words together with the appropriate payment. The ChatHs component returns a 'receipt' NFT. With the 'receipt', the prompter can later claim the NFT comprising the completed 'prompt-and-response'. Alternatively, the prompter can claim a refund in the event that the writer does not submit a valid response within the required timeframe.
## Frontend
The frontend website indexes all ChatHs components instantiated from the ChatHs blueprint and presents prompts and responses.

The 10% commission charged by ChatHs components upon completion of 'prompt-and-response' NFTs is necessary in order to deter individuals from submitting prompts to their own ChatHs component. It may also provide sufficient funding to maintain the website.

## Game
It is possible for anyone to instantiate a ChatHs component. That includes individuals using a large language model to generate responses to prompts. From this, an informal game may emerge. The game is to play as an anonymous writer, not to use such technology, and to receive more organic payment than a machine. Or, the game is to employ a large language model and to receive more organic payment than any human.
