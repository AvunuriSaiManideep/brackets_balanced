#yes
If the current character in the expression is an opening brace ( or { or [, push it into the stack.
If the current character in the expression is a closing brace ) or } or ], pop a character from the stack, and return false if the popped character is not the same as the current character, or it does not pair with the current character of the expression. Also, if the stack is empty, the total number of opening braces is less than the closing brace number at that point, so the expression cannot be balanced.
We can use a stack to solve this problem. The idea is to traverse the given expression.
The time complexity of the above solution is O(n) and requires O(n) extra space, where n is the length of the input expression.
