---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e903fabe3be75252563d80978a4aff6c8c2d2f88
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Chats["19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```