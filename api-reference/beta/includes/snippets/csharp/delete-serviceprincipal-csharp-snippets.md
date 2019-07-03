---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f879328da6bf2fda942721a62d571e879a794d2e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477280"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"]
    .Request()
    .DeleteAsync();

```