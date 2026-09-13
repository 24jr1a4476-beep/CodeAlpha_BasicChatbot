# CodeAlpha_BasicChatbot
A simple rule-based chatbot built with Python. It responds to common user inputs such as “hello,” “how are you,” and “bye” using predefined responses. This project demonstrates basic Python concepts including functions, if-elif statements, loops, and user input/output.
# Basic Rule-Based Chatbot

def chatbot_response(user_input):
    user_input = user_input.lower()

    if user_input == "hello":
        return "Hi! Nice to meet you."

    elif user_input == "how are you":
        return "I'm fine, thanks!"

    elif user_input == "what is your name":
        return "I am a simple Python chatbot."

    elif user_input == "what can you do":
        return "I can have a simple conversation with you."

    elif user_input == "bye":
        return "Goodbye!"

    else:
        return "Sorry, I don't understand that."


# Main program
print("================================")
print("       BASIC PYTHON CHATBOT")
print("================================")
print("Type 'bye' to exit the chatbot.")

while True:
    user_input = input("\nYou: ")

    response = chatbot_response(user_input)

    print("Chatbot:", response)

    if user_input.lower() == "bye":
        break

print("\nChatbot session ended.")
