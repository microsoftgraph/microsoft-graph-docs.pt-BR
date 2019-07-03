---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17f2500e14b0cbf0f0a52804fdb573ebdd85c97b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "Health Level 1",
    ClassCode = "Health 501",
    DisplayName = "Health 1",
    ExternalId = "11019",
    ExternalName = "Health Level 1",
    ExternalSource = EducationExternalSource.Sis,
    MailNickname = "fineartschool.net"
};

await graphClient.Education.Classes
    .Request()
    .AddAsync(educationClass);

```