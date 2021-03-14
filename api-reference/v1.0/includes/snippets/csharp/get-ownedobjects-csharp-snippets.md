---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7df4a487d16d9ea6519f26a936de221c7d315075
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.ServicePrincipals["{servicePrincipal-id}"].OwnedObjects
    .Request()
    .GetAsync();

```