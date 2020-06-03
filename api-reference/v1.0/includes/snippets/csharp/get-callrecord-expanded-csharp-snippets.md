---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0c0ef59e5460c0585cfdab0a76e597898ac6e31
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524613"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{id}"]
    .Request()
    .Expand("sessions($expand=segments)")
    .GetAsync();

```