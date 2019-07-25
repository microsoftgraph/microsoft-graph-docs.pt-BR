---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac7a5220305ade46784fe47cf9ca27499b8a93b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722445"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{id}"]
    .Request()
    .DeleteAsync();

```