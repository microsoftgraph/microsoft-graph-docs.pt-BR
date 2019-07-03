---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2621d5fc0bbf6b6509bcf3b340b38217354b5b19
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{object-id}"]
    .Restore()
    .Request()
    .PostAsync();

```