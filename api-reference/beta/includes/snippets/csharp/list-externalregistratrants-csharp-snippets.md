---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9644e89c477a36eb65bc3297dac73c4b57e0147
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registrants = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants
    .Request()
    .GetAsync();

```