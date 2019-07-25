---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27243f32ce1690c651ae094c08e99b2c75415507
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSku = await graphClient.SubscribedSkus["{id}"]
    .Request()
    .GetAsync();

```