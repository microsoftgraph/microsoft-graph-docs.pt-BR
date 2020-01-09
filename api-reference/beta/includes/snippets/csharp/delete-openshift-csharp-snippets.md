---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02c3f82071993cb291f23adc5de4859e5114f7d4
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40995361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.OpenShifts["{openShiftId}"]
    .Request()
    .DeleteAsync();

```