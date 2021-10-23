---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 789164fd1aac9ba4430f8b835e3ddf015929e45c
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequest = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .Request()
    .GetAsync();

```