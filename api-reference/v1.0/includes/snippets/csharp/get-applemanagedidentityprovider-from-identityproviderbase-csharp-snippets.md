---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 829261618cb3ba02837b0bcdbeef598ee04f0039
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .GetAsync();

```