---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55900a42dcba8a25f71d0f567b61c7cb6bb6e8f9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingAttendanceReport = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendanceReports["{meetingAttendanceReport-id}"]
    .Request()
    .Expand("attendanceRecords")
    .GetAsync();

```