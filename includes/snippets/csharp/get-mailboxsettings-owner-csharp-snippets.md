---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ed3eaf38bb87a4efca309807500b709bb69c02b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"]
    .Request()
    .Select("MailboxSettings")
    .GetAsync();

var mailboxSettings = users.MailboxSettings;

```