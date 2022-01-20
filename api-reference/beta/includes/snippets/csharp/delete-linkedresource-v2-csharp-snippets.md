---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d26dd2cb7da7b0992cbb4b008b957a60f9cd4f6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].LinkedResources["{linkedResource_v2-id}"]
    .Request()
    .DeleteAsync();

```