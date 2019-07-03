---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd70bdb94027d811395ee4877f513f55d6cd09d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507906"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    GivenName = "Pavel",
    Surname = "Bansky",
    EmailAddresses = new List<EmailAddress>()
    {
        new EmailAddress
        {
            Address = "pavelb@fabrikam.onmicrosoft.com",
            Name = "Pavel Bansky"
        }
    },
    BusinessPhones = new List<String>()
    {
        "+1 732 555 0102"
    }
};

await graphClient.Me.Contacts
    .Request()
    .AddAsync(contact);

```