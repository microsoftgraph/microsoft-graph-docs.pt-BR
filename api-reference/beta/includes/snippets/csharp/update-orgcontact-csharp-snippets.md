---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43f3800c9b9f8f0746ba1472612493cf136dc91f
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = new OrgContact
{
    CompanyName = "companyName-value",
    Department = "department-value",
    DisplayName = "displayName-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"businessPhones", "[\"businessPhones-value\"]"},
        {"city", "city-value"},
        {"country", "country-value"}
    }
};

await graphClient.Contacts["{id}"]
    .Request()
    .UpdateAsync(orgContact);

```