---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3370f307b43d6b390764c79aa2513285bc382d0
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806621"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].Calendar.CalendarPermissions["{id}"]
    .Request()
    .DeleteAsync();

```