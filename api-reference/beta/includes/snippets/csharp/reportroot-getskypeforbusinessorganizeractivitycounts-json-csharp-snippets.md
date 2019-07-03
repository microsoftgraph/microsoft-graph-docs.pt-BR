---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 412cd0e8241fcc316f4fc7178856e5b7e0b0e526
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityCounts = await graphClient.Reports.GetSkypeForBusinessOrganizerActivityCounts('D7')
    .Request()
    .GetAsync();

```