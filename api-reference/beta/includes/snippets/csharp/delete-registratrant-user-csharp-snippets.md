---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbff6272082a5edab452dcd9b27c80c7c9d0a418
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants["{meetingRegistrant-id}"]
    .Request()
    .DeleteAsync();

```