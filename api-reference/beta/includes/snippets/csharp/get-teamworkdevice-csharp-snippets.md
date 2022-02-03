---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0ce0f20ddff91afa6512232403066faa48f75f1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkDevice = await graphClient.Teamwork.Devices["{teamworkDevice-id}"]
    .Request()
    .GetAsync();

```