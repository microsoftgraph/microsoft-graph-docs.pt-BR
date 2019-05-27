---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b569f2fd5cc8c60c6ea814a1420d920c3c10449
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var OnlineMeeting = await graphClient.App.OnlineMeetings["{id}"]
    .Request()
    .GetAsync();

```