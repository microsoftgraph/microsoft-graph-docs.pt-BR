---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa5ff6d731072782133d6eff410a9d731b57cfe81ed8f8f410769e5e010815c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .MarkUnread(messageIds)
    .Request()
    .PostAsync();

```