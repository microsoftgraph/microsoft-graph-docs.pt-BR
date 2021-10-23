---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51daa45649379a699656a89f8e78dd22a5806edf
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistration = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .Expand("customQuestions")
    .GetAsync();

```