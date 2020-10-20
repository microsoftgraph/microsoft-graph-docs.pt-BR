---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8747b2ce8f449c7ad53685f5f8b826c09c9d221c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Request()
    .DeleteAsync();

```