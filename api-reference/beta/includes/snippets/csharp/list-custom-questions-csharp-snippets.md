---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6479a0d1ba0722920fdab44bc1987d49ce678b7a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customQuestions = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.CustomQuestions
    .Request()
    .GetAsync();

```