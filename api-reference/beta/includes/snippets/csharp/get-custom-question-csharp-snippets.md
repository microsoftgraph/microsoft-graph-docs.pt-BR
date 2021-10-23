---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7d3a004ddb876093bc286591a1c2750bc52d20e
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559079"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrationQuestion = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.CustomQuestions["{meetingRegistrationQuestion-id}"]
    .Request()
    .GetAsync();

```