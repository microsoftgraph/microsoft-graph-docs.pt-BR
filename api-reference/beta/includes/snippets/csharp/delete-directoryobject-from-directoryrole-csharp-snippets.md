---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4002b673791aebe1f85b7d5aa36c1e7d3f77ca46
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directoryroles["{id}"].Members["{id}"].Reference
    .Request()
    .DeleteAsync();

```