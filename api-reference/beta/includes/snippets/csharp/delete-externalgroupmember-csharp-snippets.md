---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10fdc5fa53e2f057437a29ab2f18945361bde6ad
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members["{externalConnectors.identity-id}"]
    .Request()
    .DeleteAsync();

```