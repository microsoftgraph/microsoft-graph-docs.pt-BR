---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a713e553250b07bfdebefa4ca269fa005044cca
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .GetFinalAttachment()
    .Request()
    .GetAsync();

```