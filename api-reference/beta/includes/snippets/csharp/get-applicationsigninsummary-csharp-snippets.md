---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9143c487bfa18897525ea7139e65df44ae584d4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAzureADApplicationSignInSummary = await graphClient.Reports.GetAzureADApplicationSignInSummary('D7')
    .Request()
    .GetAsync();

```