---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303d24a6b10ce801e1c55c278ac9da906e886bc8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Onenote.Pages["{id}"]
    .Request()
    .DeleteAsync();

```