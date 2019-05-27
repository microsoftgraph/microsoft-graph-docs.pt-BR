---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9528cdb08e2c8b5f6c3e4d8c733e11f647bab50
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    DisplayName = "Rogelio Cazares",
    GivenName = "Rogelio",
    MiddleName = "Fernando",
    Surname = "Cazares"
};

await graphClient.Education.Users["{user-id}"]
    .Request()
    .UpdateAsync(educationUser);

```