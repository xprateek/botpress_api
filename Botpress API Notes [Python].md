# Create User \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/users](https://chat.botpress.cloud/%7BwebhookUrl%7D/users)

Creates a new <ins>User</ins>. This operation can only be called when using the shared encryption key.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/users"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, headers=headers)

print(response.text)
```

# Get Or Create User \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/users/get-or-create](https://chat.botpress.cloud/%7BwebhookUrl%7D/users/get-or-create)

Get or create a new <ins>User</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/users/get-or-create"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, headers=headers)

print(response.text)
```

# Get Conversation \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{id}](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7Bid%7D)

Retrieves the <ins>Conversation</ins> object for a valid identifier.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/id"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Delete Conversation \[DELETE\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{id}](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7Bid%7D)

Permanently deletes a <ins>Conversation</ins>. It cannot be undone. Also immediately deletes corresponding <ins>Messages</ins>.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/id"

headers = {"accept": "application/json"}

response = requests.delete(url, headers=headers)

print(response.text)
```

# Create Conversation \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/conversations](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations)

Creates a new <ins>Conversation</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, headers=headers)

print(response.text)
```

# List Conversations \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/conversations](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations)

Returns a list of <ins>Conversation</ins> objects

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Get Or Create Conversation \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/get-or-create](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/get-or-create)

Get or create a new <ins>Conversation</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/get-or-create"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, headers=headers)

print(response.text)
```

# Listen Conversation \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{id}/listen](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7Bid%7D/listen)

Creates a SSE stream to receive messages and events from a conversation

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/id/listen"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# List Messages \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{conversationId}/messages](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7BconversationId%7D/messages)

Retrieves the conversation's <ins>Messages</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/conversationId/messages"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Add Participant \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{conversationId}/participants](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7BconversationId%7D/participants)

Add a <ins>Participant</ins> to a <ins>Conversation</ins>.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/conversationId/participants"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, headers=headers)

print(response.text)
```

# List Participants \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{conversationId}/participants](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7BconversationId%7D/participants)

Retrieves a list of <ins>Participants</ins> for a given <ins>Conversation</ins>.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/conversationId/participants"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Remove Participant \[DELETE\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{conversationId}/participants/{userId}](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7BconversationId%7D/participants/%7BuserId%7D)

Remove a <ins>Participant</ins> from a <ins>Conversation</ins>.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/conversationId/participants/userId"

headers = {"accept": "application/json"}

response = requests.delete(url, headers=headers)

print(response.text)
```

# Get Participant \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/conversations/{conversationId}/participants/{userId}](https://chat.botpress.cloud/%7BwebhookUrl%7D/conversations/%7BconversationId%7D/participants/%7BuserId%7D)

Retrieves a <ins>Participant</ins> from a <ins>Conversation</ins>.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/conversations/conversationId/participants/userId"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Get Message \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/messages/{id}](https://chat.botpress.cloud/%7BwebhookUrl%7D/messages/%7Bid%7D)

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/messages/id"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Delete Message \[DELETE\]

[https://chat.botpress.cloud/{webhookUrl}/messages/{id}](https://chat.botpress.cloud/%7BwebhookUrl%7D/messages/%7Bid%7D)

Permanently deletes a <ins>Message</ins>. It cannot be undone.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/messages/id"

headers = {"accept": "application/json"}

response = requests.delete(url, headers=headers)

print(response.text)
```

# Create Message \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/messages](https://chat.botpress.cloud/%7BwebhookUrl%7D/messages)

Creates a new <ins>Message</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/messages"

payload = { "payload": { "type": "audio" } }
headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, json=payload, headers=headers)

print(response.text)
```

# Get User \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/users/me](https://chat.botpress.cloud/%7BwebhookUrl%7D/users/me)

Retrieves the <ins>User</ins> object for a valid identifier.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/users/me"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Update User \[PUT\]

[https://chat.botpress.cloud/{webhookUrl}/users/me](https://chat.botpress.cloud/%7BwebhookUrl%7D/users/me)

Update <ins>User</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/users/me"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.put(url, headers=headers)

print(response.text)
```

# Delete User \[DELETE\]

[https://chat.botpress.cloud/{webhookUrl}/users/me](https://chat.botpress.cloud/%7BwebhookUrl%7D/users/me)

Permanently deletes a <ins>User</ins>. It cannot be undone.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/users/me"

headers = {"accept": "application/json"}

response = requests.delete(url, headers=headers)

print(response.text)
```

# Get Event \[GET\]

[https://chat.botpress.cloud/{webhookUrl}/events/{id}](https://chat.botpress.cloud/%7BwebhookUrl%7D/events/%7Bid%7D)

Retrieves the <ins>Event</ins> object for a valid identifier.

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/events/id"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

# Create Event \[POST\]

[https://chat.botpress.cloud/{webhookUrl}/events](https://chat.botpress.cloud/%7BwebhookUrl%7D/events)

Creates a custom <ins>Event</ins>

```python
import requests

url = "https://chat.botpress.cloud/your_default_webhook_url/events"

headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, headers=headers)

print(response.text)
```

Ref. URL : https://botpress.com/reference/introduction