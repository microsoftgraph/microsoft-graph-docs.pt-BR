---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7fd036b6ca8c408d51d4487675faf1449d8c3f05
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attendanceRecords = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendanceReports["{meetingAttendanceReport-id}"].AttendanceRecords
    .Request()
    .GetAsync();

```