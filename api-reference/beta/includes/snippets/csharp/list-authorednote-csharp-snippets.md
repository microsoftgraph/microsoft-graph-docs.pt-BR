---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54a4d2235e1686beea958e002a734a29b9d29267
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notes = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"].Notes
    .Request()
    .GetAsync();

```