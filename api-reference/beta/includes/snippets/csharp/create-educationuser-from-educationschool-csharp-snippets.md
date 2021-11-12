---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb15ca05d9f2e14b131226822034b63095f33b442a8ab67d66ab9b289b301ce8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/education/users/14008"}
    }
};

await graphClient.Education.Schools["{educationSchool-id}"].Users.References
    .Request()
    .AddAsync(educationUser);

```