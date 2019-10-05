---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5fdbf691fdeab732e5b18023bc4a4a3e86e73ce
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = await graphClient.Chats["{id}"].Messages["{id}"].HostedContents["{id}"].Content
    .Request()
    .GetAsync();

```