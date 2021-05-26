---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfabc7723af9390d0148ce3470b07e78665ba01d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"]
    .Request()
    .GetAsync();

```