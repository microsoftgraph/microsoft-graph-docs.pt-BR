---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bb60398a626844ea40921a14d2b8ab739acfdda
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690026"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["19:ea28e88c00e94c7786b065394a61f296@thread.v2"].Tabs["d731fca0-0f14-4537-971a-0ef9101ff13d"]
    .Request()
    .DeleteAsync();

```