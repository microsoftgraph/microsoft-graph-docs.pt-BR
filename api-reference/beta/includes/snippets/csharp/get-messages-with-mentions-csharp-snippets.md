---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd3644822ff96cfa052a1b4acb98f7e0a1a582f8
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Filter("MentionsPreview/IsMentioned eq true")
    .Select("subject,sender,receivedDateTime,mentionsPreview")
    .GetAsync();

```