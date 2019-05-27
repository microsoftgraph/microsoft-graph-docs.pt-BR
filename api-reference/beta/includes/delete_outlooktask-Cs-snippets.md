---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 163809b6a1186a3f5e3183893e29d1d5eacc030d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.Tasks["AAMkADIyAAAhrb_QAAA="]
    .Request()
    .DeleteAsync();

```