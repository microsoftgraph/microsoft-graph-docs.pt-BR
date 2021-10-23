---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab0d1236f8704f312086df48451479144799a454
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequests = await graphClient.Privacy.SubjectRightsRequests
    .Request()
    .GetAsync();

```