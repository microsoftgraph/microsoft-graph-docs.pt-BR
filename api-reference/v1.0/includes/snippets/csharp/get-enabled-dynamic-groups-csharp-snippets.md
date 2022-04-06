---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 793170854597bc24127b1edeeaa8133c907c8467
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var groups = await graphClient.Groups
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'")
    .Select("id,membershipRule,membershipRuleProcessingState")
    .GetAsync();

```