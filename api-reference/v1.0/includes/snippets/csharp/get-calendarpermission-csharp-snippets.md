---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee501c02f44123a6263fb28f1d9c424b6cd578e8
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806573"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = await graphClient.Users["{id}"].Calendar.CalendarPermissions["{id}"]
    .Request()
    .GetAsync();

```