---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8468e917e9b7e4b9a5a222cdf1eb40fa3f32a290bb48a25bb1b51c126c655895
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159656"
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

await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .UpdateAsync(orgContact);

```