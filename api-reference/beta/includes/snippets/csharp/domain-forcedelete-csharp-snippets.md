---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18ba187c8620a57cbe4d9c868d421eda73f915a2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["contoso.com"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```