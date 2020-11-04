---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a97e3b924e5ed0fbd191bb454358af18c3f6d36a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.ServicePrincipals["{id}"].MemberOf.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```