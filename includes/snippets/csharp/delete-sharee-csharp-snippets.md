---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1baf67e401ebe4d6a156039fd45b8933d3789c35cbfba9d033c1841e54761be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendars["AAMkADAwAABf02bAAAA="].CalendarPermissions["L289RXhjaGFuZ2VMYWJTWVnYW5C"]
    .Request()
    .DeleteAsync();

```