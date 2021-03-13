---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb0604e9aee6283380cc8638d72ac0eca4d159a6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityProviders["{identityProvider-id}"]
    .Request()
    .DeleteAsync();

```