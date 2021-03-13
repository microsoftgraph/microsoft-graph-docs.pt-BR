---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df4be4af698e0832f437b4d1a876646d943901fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{callRecords.callRecord-id}"]
    .Request()
    .Expand("sessions($expand=segments)")
    .GetAsync();

```