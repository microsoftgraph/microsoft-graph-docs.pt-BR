---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12dc129e35fc86d0a802c06c7e2a9fee8ae49a15
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443485"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Start()
    .Request()
    .PostAsync();

```