---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ec0abf1f49b6811f983dda5f078c82fe07eb63d
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attendanceReports = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendanceReports
    .Request()
    .GetAsync();

```