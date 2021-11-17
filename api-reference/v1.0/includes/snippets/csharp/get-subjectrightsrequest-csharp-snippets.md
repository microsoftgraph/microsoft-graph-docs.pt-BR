---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 789164fd1aac9ba4430f8b835e3ddf015929e45c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequest = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .Request()
    .GetAsync();

```