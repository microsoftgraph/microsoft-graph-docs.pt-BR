---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52a561ce216b261273fe50a03b812b7cd17cef04
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    RelatedContacts = new List<RelatedContact>()
    {
        new RelatedContact
        {
            DisplayName = "Father Time",
            EmailAddress = "father@time.com",
            MobilePhone = "4251231234",
            Relationship = ContactRelationship.Guardian,
            AccessConsent = true
        },
        new RelatedContact
        {
            DisplayName = "Mother Nature",
            EmailAddress = "mother@nature.co.uk",
            MobilePhone = "3251231234",
            Relationship = ContactRelationship.Parent,
            AccessConsent = true
        }
    }
};

await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .UpdateAsync(educationUser);

```