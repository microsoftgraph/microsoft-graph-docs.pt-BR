---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5440ed31d45771f32dadcd29054baeeacf3ad359
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var site = await graphClient.Sites["{site-id}"]
    .Request()
    .GetAsync();

```