---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6da78a6366f5337ff0b348d141c1c506dcae6f5b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Resources["22002"]
    .Request()
    .DeleteAsync();

```