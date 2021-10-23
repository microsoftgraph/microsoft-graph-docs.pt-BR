---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4f9f3bab746487c1aa03ec532da2b4ac01ce3be
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .GetFinalReport()
    .Request()
    .GetAsync();

```