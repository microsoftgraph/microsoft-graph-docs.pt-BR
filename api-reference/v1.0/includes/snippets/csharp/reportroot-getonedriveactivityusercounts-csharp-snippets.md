---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 861d7eb3437c759ea5f9e517ce4d50764e768271
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492102"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveActivityUserCounts('D7')
    .Request()
    .GetAsync();

```