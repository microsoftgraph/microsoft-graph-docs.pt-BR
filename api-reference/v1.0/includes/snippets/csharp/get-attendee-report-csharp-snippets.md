---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4910c660b570689456f4e061fc5a610db347fb5
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendeeReport
    .Request()
    .GetAsync();

```