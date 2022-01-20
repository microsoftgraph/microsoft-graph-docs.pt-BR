---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51daa45649379a699656a89f8e78dd22a5806edf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistration = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .Expand("customQuestions")
    .GetAsync();

```