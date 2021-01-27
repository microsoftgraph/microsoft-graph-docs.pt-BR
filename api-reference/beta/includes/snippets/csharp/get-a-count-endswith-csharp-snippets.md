---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 437834e1d4387ac703f05711a5091999bb3305e2
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("endswith(mail,'a@contoso.com'),")
    .OrderBy("userPrincipalName ")
    .GetAsync();

```