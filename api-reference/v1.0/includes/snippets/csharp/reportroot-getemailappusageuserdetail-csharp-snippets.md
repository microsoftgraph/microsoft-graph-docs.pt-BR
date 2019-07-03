---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0b1818df37fb534f6215520fd528ddf5142dfef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465681"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailAppUsageUserDetail('D7')
    .Request()
    .GetAsync();

```