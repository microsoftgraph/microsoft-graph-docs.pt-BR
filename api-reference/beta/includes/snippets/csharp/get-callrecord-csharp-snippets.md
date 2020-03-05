---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0c0ef59e5460c0585cfdab0a76e597898ac6e31
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440542"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{id}"]
    .Request()
    .Expand("sessions($expand=segments)")
    .GetAsync();

```