---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d7a51fbce4e062b7ab79a7783d078e5bad702bf
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.CustomQuestions["{meetingRegistrationQuestion-id}"]
    .Request()
    .DeleteAsync();

```