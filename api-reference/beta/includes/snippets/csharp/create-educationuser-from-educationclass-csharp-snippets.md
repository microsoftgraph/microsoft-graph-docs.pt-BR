---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6f8ae473962031bc217b08b3b003ac143bad740
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/education/users/13015"}
    }
};

await graphClient.Education.Classes["11011"].Members.References
    .Request()
    .AddAsync(educationUser);

```