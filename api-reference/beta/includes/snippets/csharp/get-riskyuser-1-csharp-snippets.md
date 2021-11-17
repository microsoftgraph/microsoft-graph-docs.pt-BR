---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f916aa7ab57ea75c968f27afd0ba436f7d0e5c46d9d1c142047c4e4f2e80bd82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUser = await graphClient.RiskyUsers["{riskyUser-id}"]
    .Request()
    .GetAsync();

```