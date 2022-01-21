---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8ba5d61eddbdefae56e1a47334b4a61b5d57ff9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"]
    .Request()
    .DeleteAsync();

```