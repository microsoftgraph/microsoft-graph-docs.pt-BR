---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3528d11e577d12991ac33dca491ee960b688979aa4d20554bf577a573f3ab1c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ClaimsMappingPolicies["{claimsMappingPolicy-id}"]
    .Request()
    .DeleteAsync();

```