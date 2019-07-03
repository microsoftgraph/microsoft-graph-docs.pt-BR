---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac7a5220305ade46784fe47cf9ca27499b8a93b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{id}"]
    .Request()
    .DeleteAsync();

```