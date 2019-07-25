---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14c1e49a15c1a7a6ea4ec47f318f826370743e82
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Groups["{id}"].Owners
    .Request()
    .GetAsync();

```