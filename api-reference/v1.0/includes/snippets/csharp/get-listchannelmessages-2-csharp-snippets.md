---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbe23dcf24173f28cc5009d62c8db7474babc7de
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .Top(3)
    .GetAsync();

```