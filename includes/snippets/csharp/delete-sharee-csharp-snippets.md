---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91d6a53badffede7af60a23ec63e7cb34af19a73
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendars["AAMkADAwAABf02bAAAA="].CalendarPermissions["L289RXhjaGFuZ2VMYWJTWVnYW5C"]
    .Request()
    .DeleteAsync();

```