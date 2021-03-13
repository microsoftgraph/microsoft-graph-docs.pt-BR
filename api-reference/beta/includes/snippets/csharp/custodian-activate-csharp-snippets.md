---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d01512f2269d318b7e86f685e079a5906f4fd5bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784616"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"]
    .Activate()
    .Request()
    .PostAsync();

```