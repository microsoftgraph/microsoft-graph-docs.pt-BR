---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c64d16b6bed0d40c7ac38ca37be5acec3ebc18a8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "submissions")
};

var assignments = await graphClient.Education.Users["{educationUser-id}"].Assignments
    .Request( queryOptions )
    .GetAsync();

```