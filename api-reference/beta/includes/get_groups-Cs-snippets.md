---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33cb6e273c28aeb549ba88cfce8433a6e9eaf64e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .GetAsync();

```