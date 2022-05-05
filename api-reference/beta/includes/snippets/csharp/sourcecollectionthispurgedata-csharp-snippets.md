---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81ac7e6a948cfd615b47edf1dc5d4b75102b2721
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211418"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .PurgeData()
    .Request()
    .PostAsync();

```