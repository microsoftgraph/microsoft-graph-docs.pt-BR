---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4339290fb3088533677cb5e3132696f3e34cc761
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Patents["{itemPatent-id}"]
    .Request()
    .DeleteAsync();

```