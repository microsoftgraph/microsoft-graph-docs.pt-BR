---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2052b4991983d5ed3a422f224f2935ab495b964
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = await graphClient.Security.SecureScoreControlProfiles["{id}"]
    .Request()
    .GetAsync();

```