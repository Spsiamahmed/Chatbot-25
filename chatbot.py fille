from chatterbot import ChatBot
from chatterbot.trainers import ChatterBotCorpusTrainer

# চ্যাটবট তৈরি
chatbot = ChatBot('MyChatBot')

# ট্রেনিং সেটআপ
trainer = ChatterBotCorpusTrainer(chatbot)

# বাংলা কোরপাসে ট্রেনিং দিন
trainer.train('chatterbot.corpus.bengali')

# চ্যাটবটের সাথে কথোপকথন
while True:
    try:
        user_input = input("আপনি: ")
        if user_input.lower() == 'exit':
            break
        response = chatbot.get_response(user_input)
        print("চ্যাটবট: ", response)
    except (KeyboardInterrupt, EOFError, SystemExit):
        break
