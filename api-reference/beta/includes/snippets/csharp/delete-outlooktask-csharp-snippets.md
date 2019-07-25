---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 163809b6a1186a3f5e3183893e29d1d5eacc030d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.Tasks["AAMkADIyAAAhrb_QAAA="]
    .Request()
    .DeleteAsync();

```