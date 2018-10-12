# blockchain
Building a blockchain with python
class Blockchain(object):
    def __init__(self):
        self.chain = []
        self.current_transactions = []

    def new_block(self):
        # creates a new block and adds it to the chain
        pass

    def new_transaction(self):
        # Add new transactions to the list of transactions
        pass

    @staticmethod
    def hash(block):
        # Hashes a block
        pass

    @property
    def last_block(self):
        # Returns the last Block in the chain
        pass

class Blockchain(object):
    ...


    def new_transaction(self, sender, recipient, amount):
        """"""
        Creates a new transaction to go into the next mined Blockchain

        :param sender: <str> Address of the sender
        :param recipient: <str> Address of the Recipient
        :param amount: <int> amount
        :return: <int> The index of the Block that willl hold the transaction
        """"""

        self.current_transactions.append({
            'sender': sender,
            'recipient': recipient,
            'amount': amount,
        })
        return self.last_block['index'] + 1

import hashlib
import json
from time import time

class Blockchain(object):
    def __init__(self):
        self.current_transactions = []
        self.chain = []
