---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38cf36e48906fa5d668d1d597321e0870aa897b0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    DisplayName = "Dion Matheson",
    GivenName = "Dion",
    MiddleName = null,
    Surname = "Matheson",
    Mail = "DionM@contoso.com",
    MobilePhone = "+1 (253) 555-0101",
    CreatedBy = new IdentitySet
    {
        User = new Identity
        {
            DisplayName = "Susana Rocha",
            Id = "14012"
        }
    },
    ExternalSource = EducationExternalSource.Sis,
    MailingAddress = new PhysicalAddress
    {
        City = "Los Angeles",
        CountryOrRegion = "United States",
        PostalCode = "98055",
        State = "CA",
        Street = "12345 Main St."
    },
    PrimaryRole = EducationUserRole.Student,
    ResidenceAddress = new PhysicalAddress
    {
        City = "Los Angeles",
        CountryOrRegion = "United States",
        PostalCode = "98055",
        State = "CA",
        Street = "12345 Main St."
    }
};

await graphClient.Education.Users
    .Request()
    .AddAsync(educationUser);

```