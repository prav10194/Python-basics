## Basics

<b>1. re.sub(pattern, repl, string, count=0, flags=0)</b>
   <br/><br/>pattern -> regex pattern
   <br/>repl -> chracter/string to be replaced with
   <br/>string -> the input text
   <br/>count (optional) -> number of times the regex will be run - defaulted to all occurrences 
   <br/>flags (optional) -> refer this https://pynative.com/python-regex-flags/ 



## Few examples of various regex usecases

<b>1. Removing all alphanumeric characters from string</b>

```python
palindrome = "A man, a plan, a canal: Panama"
result = re.sub(r'[^A-Za-z0-9]', '', palindrome) # prints out AmanaplanacanalPanama

# or if using flags
result = re.sub(r'[^a-z0-9]', '', palindrome, flags=re.IGNORECASE)

```

