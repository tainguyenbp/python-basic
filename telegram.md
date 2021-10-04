### install pip
```
pip install telethon
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
