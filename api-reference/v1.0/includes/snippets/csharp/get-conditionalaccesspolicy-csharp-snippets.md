---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80d6b2c6058e9c95842e274afb7395242c79d204f8ef3d75bb4817c2fde69380
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329481"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = await graphClient.Identity.ConditionalAccess.Policies["{conditionalAccessPolicy-id}"]
    .Request()
    .GetAsync();

```