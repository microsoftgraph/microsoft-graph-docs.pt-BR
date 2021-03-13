---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e87b083f26de185099f61c9fed177283aee30a66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{callRecords.callRecord-id}"].Sessions
    .Request()
    .Expand("segments")
    .GetAsync();

```