---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f82253a9feb233ee0042c3928cdcf3c593051e51
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailActivityCounts('D7')
    .Request()
    .GetAsync();

```