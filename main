import discord
import aiohttp
from keep_alive import keep_alive




#Be sure to enter the url the consol gives you, more on that in README



bot=client #if you're defining client to start 

client=bot #if you're defining bot to start 

@client.event
async def on_ready():
    print('Bot is online!')
    alive_status.start()

@tasks.loop(seconds=1)
async def alive_status():
  session = aiohttp.ClientSession()
  await session.get('https://sentry.replit.com/api/10/security/?sentry_key=615192fd532445bfbbbe966cd7131791')
  await session.get('https://exactreplitbotname.exactreplitusername.repl.co')
  print(session)
  await session.close()
  

keep_alive()
bot.run(os.getenv("TOKEN"))
