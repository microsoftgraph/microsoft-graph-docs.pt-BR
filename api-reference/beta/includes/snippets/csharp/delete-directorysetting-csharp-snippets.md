---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d898d15e5529c6dd93e293b79ffc7273a8e90343
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Settings["{id}"]
    .Request()
    .DeleteAsync();

```