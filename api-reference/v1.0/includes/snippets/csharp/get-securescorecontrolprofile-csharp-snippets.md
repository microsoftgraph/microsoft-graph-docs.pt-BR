---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2052b4991983d5ed3a422f224f2935ab495b964
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = await graphClient.Security.SecureScoreControlProfiles["{id}"]
    .Request()
    .GetAsync();

```