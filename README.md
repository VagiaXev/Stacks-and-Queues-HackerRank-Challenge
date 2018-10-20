# Stacks-and-Queues-HackerRank-Challenge
Determine if a given string is a palindrome or not 

A palindrome is a word, phrase, number, or other sequence of characters which reads the same backwards and forwards. Can you determine if a given string, , is a palindrome?

To solve this challenge, we create a class named Solution that includes the following declarations and implementations: 

1. Two instance variables: one for your , and one for your .
2. A void pushCharacter(char ch) method that pushes a character onto a stack.
3. A void enqueueCharacter(char ch) method that enqueues a character in the  instance variable.
4. A char popCharacter() method that pops and returns the character at the top of the  instance variable.
5. A char dequeueCharacter() method that dequeues and returns the first character in the  instance variable.

class Solution:
    # Write your code here
    def __init__(self):
        self.stack = []
        self.queue = []

    # Method to push the characters of the string onto stack
    def pushCharacter(self,item):
        self.stack.append(item) 

    # Method to enqueue the characters of the string into a queue data structure
    def enqueueCharacter(self, item):
        self.queue.insert(0,item)
        
    # Method that pops and returns the character at the top of the stack instance variable 
    def popCharacter(self):
        return self.stack.pop()
    
    # Method that dequeues and returns the first character in the queue instance variable 
    def dequeueCharacter(self):
        return self.queue.pop()
