---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e79ea48acdd97930128a36235dd995841e3370cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityMinuteCounts = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```