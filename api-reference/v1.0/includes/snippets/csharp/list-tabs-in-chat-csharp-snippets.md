---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5372f35c0356c4ab1a44c72326fedf60166b304
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954881"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Chats["{chat-id}"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```