---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee8382fe1ebe71db13d474c310600dca961bf09d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessOrganizerActivityCounts('D7')
    .Request()
    .GetAsync();

```