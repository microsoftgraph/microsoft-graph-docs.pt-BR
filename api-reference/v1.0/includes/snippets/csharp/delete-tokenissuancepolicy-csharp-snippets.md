---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66e7885011d565456d36165cb4da8b5b833cd7028693c550f431efcbb39cb68b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.TokenIssuancePolicies["{tokenIssuancePolicy-id}"]
    .Request()
    .DeleteAsync();

```