---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6df7ec9dfc1de8d9df674b8686d3c7a3dbd4ecc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.TokenIssuancePolicies["{tokenIssuancePolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```