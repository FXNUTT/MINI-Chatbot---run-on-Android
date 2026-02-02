print(" Mini Chatbot")
print("Type 'exit' to quit\n")

chat_count = 0

while True:
    user_input = input("You: ").lower()
    chat_count += 1

    if user_input == "exit":
        print("Bot: Bye! We talked", chat_count - 1, "times ")
        break

    elif user_input in ["hi", "hello", "hey"]:
        print("Bot: Hi! Nice to meet you ")

    elif "name" in user_input:
        print("Bot: I'm a Mini Chatbot written in Python.")

    elif "help" in user_input:
        print("Bot: Try saying hello, asking my name, or type exit.")

    else:
        print("Bot: Sorry, I don't understand yet")
