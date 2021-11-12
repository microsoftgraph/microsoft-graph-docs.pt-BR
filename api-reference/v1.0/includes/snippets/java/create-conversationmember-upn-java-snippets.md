---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af4c7c6fe57039d8cb8d24ce4be3820f468d4823
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;
conversationMember.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"));

graphClient.teams("ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062").members()
    .buildRequest()
    .post(conversationMember);

```