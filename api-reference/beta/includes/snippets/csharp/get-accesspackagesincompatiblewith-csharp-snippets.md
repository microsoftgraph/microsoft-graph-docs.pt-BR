---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 601a59e543dab990101f5036fa45c73f0b2fccf4c300b91ecc4c4a708d14c5c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackagesIncompatibleWith = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].AccessPackagesIncompatibleWith
    .Request()
    .GetAsync();

```