---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 705841f2c295ca2f4667a9b99f189e510b9891a2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants["{meetingRegistrantBase-id}"]
    .Request()
    .DeleteAsync();

```