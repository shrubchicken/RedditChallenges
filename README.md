# RedditChallenges
These are my solutions to programming challenges I find on Reddit. They aren't always the most efficient solutions,
but they are my own. I try to write tons of comments to help others understand. 

I'm also not necessarily looking for the most efficient answer anyway. I'm a hobbyist programmer and try to have fun
with the stuff I write. 

# UPC Generator and Checker
This program is self-explanatory. It will either generate a random 12-digit UPC when asked or verify a 12-digit UPC by calculating and comparing the check (final) digit. This combined both a beginner and intermediate Reddit challenge into a single program. One challenge was computing just the final digit given 11 characters, and the other was generating an entire UPC from scratch. 

The Luhn Algorithm for UPCs is pretty straightforward, and doesn't really require much except for the check-digit to be a multiple of ten. The sequence of digits prior to that check digit can be any combination, but the check digit itself is computed in a particular manner based on those digits. For example, you sum the odd and even indexes independently, but thanks to computing we can do that independently within the same loop. There is unfortunately some redundancy due to how I handled the Luhn Algorithm and the speed at which I completed this challenge. However, it does include recursion which I feel should count for something and I did warn you that my solutions will not always be pretty.

# Addititive Persistence
The addititive persistence of a value is the amount of times you can add all the single integers in the value to reach a single digit. I kinda wanna revisit this program at some point and make it prettier now that I explain that.

# Balanced/Balanced Bonus
This program just checked to make sure that characters in a given string appear in the string an equal amount of times. First it started with x and y and the bonus includes all lowercase characters in the English alphabet.