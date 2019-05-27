---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1466a92c760441182fda7bcd88b3548f4a7281c3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembers = await graphClient.AdministrativeUnits["{id}"].ScopedRoleMembers
    .Request()
    .GetAsync();

```