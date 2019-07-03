---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75de1e525afafa27ef985c467226d3e9100c5897
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScores = await graphClient.Security.SecureScores
    .Request()
    .Top(1)
    .GetAsync();

```