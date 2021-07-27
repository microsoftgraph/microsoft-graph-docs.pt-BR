---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55336fbba8544dd7f9d9fa9f2a5895aaeba63ab6
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectionOperation = await graphClient.Connections["{externalConnectors.externalConnection-id}"].Operations["{externalConnectors.connectionOperation-id}"]
    .Request()
    .GetAsync();

```