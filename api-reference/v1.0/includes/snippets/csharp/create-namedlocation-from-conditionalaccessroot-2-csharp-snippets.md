---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edc31e603c1d0efa700dc5b882c3e77d3b4de66e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new CountryNamedLocation
{
    DisplayName = "Named location with unknown countries and regions",
    CountriesAndRegions = new List<String>()
    {
        "US",
        "GB"
    },
    IncludeUnknownCountriesAndRegions = true
};

await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .AddAsync(namedLocation);

```