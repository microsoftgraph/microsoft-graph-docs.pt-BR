---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6479a0d1ba0722920fdab44bc1987d49ce678b7a
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customQuestions = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.CustomQuestions
    .Request()
    .GetAsync();

```