---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29e14f55a1676e2417668b8b201fc19184087694
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserDetail = await graphClient.Reports.GetTeamsDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```