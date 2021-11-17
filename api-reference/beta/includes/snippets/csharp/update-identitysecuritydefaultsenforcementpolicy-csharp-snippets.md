---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 785ba2e305c2ab8e30e618bccc2ad088498c69d481e907f0fcc25ea78bcc254d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identitySecurityDefaultsEnforcementPolicy = new IdentitySecurityDefaultsEnforcementPolicy
{
    IsEnabled = false
};

await graphClient.Policies.IdentitySecurityDefaultsEnforcementPolicy
    .Request()
    .UpdateAsync(identitySecurityDefaultsEnforcementPolicy);

```