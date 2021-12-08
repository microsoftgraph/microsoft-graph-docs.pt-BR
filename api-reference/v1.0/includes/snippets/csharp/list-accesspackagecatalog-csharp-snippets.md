---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfe5b85322800fbb5aba93865b153e8b3ed0115a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var catalogs = await graphClient.IdentityGovernance.EntitlementManagement.Catalogs
    .Request()
    .GetAsync();

```