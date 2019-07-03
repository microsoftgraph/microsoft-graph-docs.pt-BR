---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 460bc93c7e2ebcde55a74533e6849be06b62958d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScore = await graphClient.Security.SecureScores["{id}"]
    .Request()
    .GetAsync();

```