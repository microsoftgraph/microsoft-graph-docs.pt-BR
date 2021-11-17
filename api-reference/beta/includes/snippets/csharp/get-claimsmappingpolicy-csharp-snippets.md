---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de0ef91fa6912391ef3b9ccd02b52bb45a3d18113c3a871e5da42aaccd838834
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = await graphClient.Policies.ClaimsMappingPolicies["{claimsMappingPolicy-id}"]
    .Request()
    .GetAsync();

```