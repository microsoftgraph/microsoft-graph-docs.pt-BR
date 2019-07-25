---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d898d15e5529c6dd93e293b79ffc7273a8e90343
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Settings["{id}"]
    .Request()
    .DeleteAsync();

```