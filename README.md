
# SCRIPT

The ability to lock and unlock coins is at the heart of what it means to transfer Bitcoin.

### Mechanics of SCRIPT

If you are confused about what a "smart contract" is, don't worry. "Smart contract" is a fancy way of saying "programmable" and the "smart contract language" is simply a programming language. SCRIPT is the smart contract langauge, or the programming language used to express how bitcoins are to be transferred.

Think of a personal check. In a sense, a personal check is a type of contract. A personal check is an agreement to transfer some amount of money from one person to another. Bitcoin has the digital equivalent of a contract in SCRIPT.

SCRIPT is a limited programming language in the sense that it doesn't have certain features. Specifically, it does not have any mechanism for loops and is not Turing complete.

What you are required to do as part of a transaction is to assign Bitcoins to a *locking* script. The locking script is what's specified in ScriptPubKey (see chapter 5). Think of this as the locked box where some money is deposited which only the person with the key to the box can open. The money inside, of course, can only be accessed by someone with the key.

The actual unlocking of bitcoin is done in the ScriptSig field and proves ownership of the locked box in order to spend the funds.

### Try it

Determine a ScriptSig that will satisfy this scriptPubKey:

```
767695935687
```

#### Hint: use the Script.parse method


```python
from script import Script

hex_script = '767695935687'

# bytes.fromhex the script
# parse the script
```
