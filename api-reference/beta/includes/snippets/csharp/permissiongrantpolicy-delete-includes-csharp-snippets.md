---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa114e2f36b7e5ed0917654b2794464ce75fa4d114c620f15aebcb7513472010
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes["{permissionGrantConditionSet-id}"]
    .Request()
    .DeleteAsync();

```