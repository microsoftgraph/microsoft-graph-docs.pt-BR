---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15e866888e6cf8bc82548038f497f7315b8d78d2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{caseId}"].Custodians["{custodianId}"].UnifiedGroupSources["{unifiedGroupSourceId}"]
    .Request()
    .DeleteAsync();

```