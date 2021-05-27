---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b62f699c134b5f16369ca341d35b19968bdd7c11
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .DeleteAsync();

```