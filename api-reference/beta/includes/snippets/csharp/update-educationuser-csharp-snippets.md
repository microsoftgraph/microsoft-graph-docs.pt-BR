---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c2ef9fb22dbd6ba3accd317714066f9ae2f8e38
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714312"
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

await graphClient.Education.Users["13020"]
    .Request()
    .UpdateAsync(educationUser);

```