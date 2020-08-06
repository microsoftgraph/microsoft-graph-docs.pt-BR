---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ed7922f83b6ca480e80cfc1e88e34afd913fc3a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567089"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new CountryNamedLocation
{
    DisplayName = "Updated named location without unknown countries and regions",
    CountriesAndRegions = new List<String>()
    {
        "CA",
        "IN"
    },
    IncludeUnknownCountriesAndRegions = false
};

await graphClient.Identity.ConditionalAccess.NamedLocations["1c4427fd-0885-4a3d-8b23-09a899ffa959"]
    .Request()
    .UpdateAsync(namedLocation);

```