---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2621d5fc0bbf6b6509bcf3b340b38217354b5b19
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605170"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{object-id}"]
    .Restore()
    .Request()
    .PostAsync();

```