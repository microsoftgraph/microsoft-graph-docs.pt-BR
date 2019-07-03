---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 636008c94ea5c339accc3645164b521eb76c1e2c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35462976"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageMailboxCounts('D7')
    .Request()
    .GetAsync();

```