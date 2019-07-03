---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5757aa0abcca21238914310f22a2062bb3d42a86
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReplyAll()
    .Request()
    .PostAsync();

```