---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4f33dd563acff18ea7e8bbb7c3c8ae200c6b4b3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistration = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .GetAsync();

```