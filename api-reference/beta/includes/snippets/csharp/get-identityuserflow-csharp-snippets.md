---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc198ec79a87427430d44f377823716d4344498c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = await graphClient.Identity.UserFlows["{identityUserFlow-id}"]
    .Request()
    .GetAsync();

```