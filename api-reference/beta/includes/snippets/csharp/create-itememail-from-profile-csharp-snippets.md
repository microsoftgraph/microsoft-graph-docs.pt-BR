---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5fdac2eb6d8b4229052c2a58eabc36be1b924cf
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = new ItemEmail
{
    Address = "Innocenty.Popov@adventureworks.com"
};

await graphClient.Me.Profile.Emails
    .Request()
    .AddAsync(itemEmail);

```