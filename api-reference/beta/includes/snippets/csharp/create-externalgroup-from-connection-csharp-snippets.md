---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23fd5f9450dfb2112b80d0f6921e896534008a43
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573082"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroup = new ExternalGroup
{
    Id = "31bea3d537902000",
    DisplayName = "Contoso Marketing",
    Description = "The product marketing team"
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups
    .Request()
    .AddAsync(externalGroup);

```