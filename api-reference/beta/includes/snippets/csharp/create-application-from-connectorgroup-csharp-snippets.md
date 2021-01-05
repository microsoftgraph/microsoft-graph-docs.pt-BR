---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 749c6796473462d7bca4a6d1f0e863eed1af78b3
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752834"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].ConnectorGroup.Reference
    .Request()
    .PutAsync("{id}");

```