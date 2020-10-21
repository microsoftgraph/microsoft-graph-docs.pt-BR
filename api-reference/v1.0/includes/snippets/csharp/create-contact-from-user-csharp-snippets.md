---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd70bdb94027d811395ee4877f513f55d6cd09d0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606354"
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