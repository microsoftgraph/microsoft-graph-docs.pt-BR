---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9f82f7454477c3c78bfb59526b4a496c5c18f8b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identity = new Microsoft.Graph.ExternalConnectors.Identity
{
    Id = "e5477431-1038-484e-bf69-1dfedb97a110",
    Type = Microsoft.Graph.ExternalConnectors.IdentityType.Group
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(identity);

```