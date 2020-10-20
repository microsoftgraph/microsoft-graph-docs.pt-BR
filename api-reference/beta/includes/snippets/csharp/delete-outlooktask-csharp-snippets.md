---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 163809b6a1186a3f5e3183893e29d1d5eacc030d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.Tasks["AAMkADIyAAAhrb_QAAA="]
    .Request()
    .DeleteAsync();

```