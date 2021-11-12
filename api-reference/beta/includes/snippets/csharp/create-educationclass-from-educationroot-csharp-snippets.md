---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adad9a966292eb903d0509ad90480171deca09287f79df43e9e8faae11573b70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156801"
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