---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e6743364a59f35d966e2c04814ec3ed77b2e4b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = new BookingBusiness
{
    DisplayName = "Fourth Coffee",
    Address = new PhysicalAddress
    {
        Type = PhysicalAddressType.Unknown,
        PostOfficeBox = "P.O. Box 123",
        Street = "4567 Main Street",
        City = "Buffalo",
        State = "NY",
        CountryOrRegion = "USA",
        PostalCode = "98052"
    },
    Phone = "206-555-0100",
    Email = "manager@fourthcoffee.com",
    WebSiteUrl = "https://www.fourthcoffee.com",
    DefaultCurrencyIso = "USD"
};

await graphClient.BookingBusinesses
    .Request()
    .AddAsync(bookingBusiness);

```