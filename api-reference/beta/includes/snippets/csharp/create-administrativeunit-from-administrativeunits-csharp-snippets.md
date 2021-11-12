---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d74fdadaebd7efc6eb48ef8a35cc90854a21315d7a7f17404b2c5d4c7a6264e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898078"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "Seattle District Technical Schools",
    Description = "Seattle district technical schools administration",
    Visibility = "HiddenMembership"
};

await graphClient.AdministrativeUnits
    .Request()
    .AddAsync(administrativeUnit);

```