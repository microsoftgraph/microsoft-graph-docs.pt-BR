---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14fa540167cdcbe951f664451ae739ec3d959e8c1d805e56b178d72c547fa7f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "displayName-value",
    Description = "description-value",
    Visibility = "visibility-value"
};

await graphClient.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .UpdateAsync(administrativeUnit);

```