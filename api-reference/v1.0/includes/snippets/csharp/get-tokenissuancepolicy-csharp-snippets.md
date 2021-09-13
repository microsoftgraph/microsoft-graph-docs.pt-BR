---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8ef7877e30e7d7567f512629c4d78bae194121b64b8b461e082294f89dd321f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100593"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = await graphClient.Policies.TokenIssuancePolicies["{tokenIssuancePolicy-id}"]
    .Request()
    .GetAsync();

```