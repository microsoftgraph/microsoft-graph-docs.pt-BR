---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d36512505ec5170018fb38acb0eb7a40476d05d4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResources = await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"].LinkedResources
    .Request()
    .GetAsync();

```