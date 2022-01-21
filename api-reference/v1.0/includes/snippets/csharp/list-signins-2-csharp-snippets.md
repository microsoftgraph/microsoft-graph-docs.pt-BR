---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe7d9501989ba5327d6d7174e6df057fb8caa602
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("top", "10")
};

var signIns = await graphClient.AuditLogs.SignIns
    .Request( queryOptions )
    .Filter("startsWith(appDisplayName,'Graph')")
    .GetAsync();

```