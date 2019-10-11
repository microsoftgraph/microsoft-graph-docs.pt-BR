---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00ac09f7c19c9ba5b3b432fb0c2d79a215571c59
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Chats["{id}"].Messages["{id}"].HostedContents["{id}"].Content
    .Request()
    .GetAsync();

```