---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4330278352fb61fca76bd59c78a1e0b456e22686
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var submissions = await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions
    .Request()
    .GetAsync();

```