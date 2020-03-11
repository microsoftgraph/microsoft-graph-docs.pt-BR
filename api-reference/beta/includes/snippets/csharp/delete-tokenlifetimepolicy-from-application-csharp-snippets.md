---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fec7262a430de0a0f4208d46bf135c283ecf4c8c
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].TokenLifetimePolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```