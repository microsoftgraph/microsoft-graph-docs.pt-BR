---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a7a517483ba57a9aa98e69fc400ea95c8dffcde
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "displayName-value",
    Description = "description-value",
    Visibility = "visibility-value"
};

await graphClient.AdministrativeUnits["{id}"]
    .Request()
    .UpdateAsync(administrativeUnit);

```