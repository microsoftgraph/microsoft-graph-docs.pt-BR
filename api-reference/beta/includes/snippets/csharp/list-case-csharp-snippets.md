---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea9a14d4b18b244c215c0436b1e375a5834f3c00eacb755a913c377cf96dfbad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cases = await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .GetAsync();

```