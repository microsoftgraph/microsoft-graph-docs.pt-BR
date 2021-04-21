---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3956dd2ea9400d3ed42916518f6aab25d9f4f1b0
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920401"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingAttendanceReport = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].MeetingAttendanceReport
    .Request()
    .GetAsync();

```