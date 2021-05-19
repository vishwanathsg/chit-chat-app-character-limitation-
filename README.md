# chit-chat-app-character-limitation-
This code is based upon character limitation like in twitter

def char_list(char_input):
    x=list(char_input) #Used list to convert the string into individual characters (includes spaces)

    if len(list(char_input)) > 200: #Made a condition to check whether the individual characters are more than or  less than 200 chars
        print()
        print("Result =",char_input[0:200]) #Removed "list()" in order to print whole words, and set the range [0:n-1] = [0:200-1] = first 200 words

    else:
        print()
        print("Result =",char_input) #If characters < 200, then directly print the input string

    return(x)

char_input=str(input("Enter the text you want to send: "))
char_list(char_input)
