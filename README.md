# Dynamo1
import telebot

bot = telebot.TeleBot("5132150480:AAH7WFCVt1hJrzWYSphQxhXG7NDWwpD7Zks")

@bot.message_handler(commands=['start'])
def start(message):
  bot.send_message(message.chat.id, 'Саламалейкум', parse_mode='html')


bot.polling(none_stop=True)
