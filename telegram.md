### install pip
```
pip install telethon

https://api.telegram.org/botAPITOKENNUMBER:APITOKENKEYHERE/sendmessage?chat_id=-100GROUPNUMBER&text=test

https://api.telegram.org/botXXX:YYYY/getUpdates

https://api.telegram.org/bot<YourBOTToken>/getUpdates
 
https://api.telegram.org/bot123456789:jbd78sadvbdy63d37gda37bd8/getUpdates

curl -X POST "https://api.telegram.org/botXXX:YYYY/sendMessage" -d "chat_id=-zzzzzzzzzz&text=my sample text"

```

### telegram
```
from telethon import InteractiveTelegramClient
from telethon.utils.tl_utils import get_display_name

client = InteractiveTelegramClient('session_id', 'YOUR_PHONE_NUMBER', api_id=1234YOURAPI_ID, api_hash='YOUR_API_HASH')

dialog_count = 10
dialogs, entities = client.get_dialogs(dialog_count)
for i, entity in enumerate(entities):
                    i += 1  # 1-based index
                    print('{}. {}. id: {}'.format(i, get_display_name(entity), entity.id))
```
