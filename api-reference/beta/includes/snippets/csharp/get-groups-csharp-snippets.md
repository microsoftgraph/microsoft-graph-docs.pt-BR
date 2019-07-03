---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33cb6e273c28aeb549ba88cfce8433a6e9eaf64e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .GetAsync();

```