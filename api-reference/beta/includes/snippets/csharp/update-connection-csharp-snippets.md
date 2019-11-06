---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1d6c4dd06099c2157d3a41f0068f26a3ddc4b58
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = new ExternalConnection
{
    Name = "Contoso HR Service Tickets",
    Description = "Connection to index HR service tickets"
};

await graphClient.Connections["contosohr"]
    .Request()
    .UpdateAsync(externalConnection);

```