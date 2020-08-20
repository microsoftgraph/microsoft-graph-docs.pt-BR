---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d55dc5861c9b86c552efb14a87d548ae98414fa4
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = new WorkPosition
{
    Detail = new PositionDetail
    {
        Company = new CompanyDetail
        {
            DisplayName = "Adventureworks Ltd.",
            Department = "Consulting",
            OfficeLocation = "AW23/344",
            Address = new PhysicalAddress
            {
                Type = PhysicalAddressType.Business,
                Street = "123 Patriachy Ponds",
                City = "Moscow",
                CountryOrRegion = "Russian Federation",
                PostalCode = "RU-34621"
            },
            WebUrl = "https://www.adventureworks.com"
        },
        JobTitle = "Senior Product Branding Manager II",
        Role = "consulting"
    },
    IsCurrent = true
};

await graphClient.Me.Profile.Positions
    .Request()
    .AddAsync(workPosition);

```