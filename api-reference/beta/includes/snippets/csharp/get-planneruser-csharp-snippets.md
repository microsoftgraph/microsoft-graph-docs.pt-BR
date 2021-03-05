---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56df01b9e48acb03cb3ac457f7366ffae0187e1e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerUser = await graphClient.Me.Planner
    .Request()
    .GetAsync();

```