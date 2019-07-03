---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2216615d76ce96277f66e05536975f5a227f9d5a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Applications.Delta()
    .Request()
    .GetAsync();

```