---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faedc0e173d1f17615bf34d684dfc8e83bfa0285
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    CustomSecurityAttributes = new CustomSecurityAttributeValue
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"Engineering", "{\"@odata.type\":\"#Microsoft.DirectoryServices.CustomSecurityAttributeValue\",\"ProjectDate\":\"2022-10-01\"}"}
        }
    }
};

await graphClient.Users["{user-id}"]
    .Request()
    .UpdateAsync(user);

```