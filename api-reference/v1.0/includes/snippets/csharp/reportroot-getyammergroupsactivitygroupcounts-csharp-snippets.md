---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec38d005bef75ce6eefec1ffb3b358899fe653de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerGroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```