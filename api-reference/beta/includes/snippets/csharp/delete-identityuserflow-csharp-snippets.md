---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 601c152fd3e8ef02ffa1bce4c91b571481607729
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlows["{identityUserFlow-id}"]
    .Request()
    .DeleteAsync();

```