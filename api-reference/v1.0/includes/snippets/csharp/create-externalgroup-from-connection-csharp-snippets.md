---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10ed52aec7c5e7e9c8c87571306832140217dad8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroup = new Microsoft.Graph.ExternalConnectors.ExternalGroup
{
    Id = "31bea3d537902000",
    DisplayName = "Contoso Marketing",
    Description = "The product marketing team"
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups
    .Request()
    .AddAsync(externalGroup);

```