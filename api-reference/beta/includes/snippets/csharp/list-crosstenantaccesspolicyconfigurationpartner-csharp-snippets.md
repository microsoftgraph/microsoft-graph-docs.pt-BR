---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ddfa3d2688f0c8c5d331dab2e1b157435cc3482
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336547"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var partners = await graphClient.Policies.CrossTenantAccessPolicy.Partners
    .Request()
    .GetAsync();

```