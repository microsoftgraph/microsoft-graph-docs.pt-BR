---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df402d5587c9d0b9499185f8e6288427272821ec62303fc39fe8a12d4671d229
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = new Microsoft.Graph.ExternalConnectors.ExternalConnection
{
    Id = "contosohr",
    Name = "Contoso HR",
    Description = "Connection to index Contoso HR system"
};

await graphClient.External.Connections
    .Request()
    .AddAsync(externalConnection);

```