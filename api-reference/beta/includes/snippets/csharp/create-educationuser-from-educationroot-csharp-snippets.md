---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfa55ce7efc5d62582db98d807088b0bdc8713cd244f50343d0d76d7a8640d5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101752"
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