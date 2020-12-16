---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a34ac9cc36d92c75bd7aa90aa3c6085594a6189
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692820"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = new Case
{
    DisplayName = "My Case 1 - Renamed",
    Description = "Updated description",
    ExternalId = "Updated externalId"
};

await graphClient.Compliance.Ediscovery.Cases["061b9a92-8926-4bd9-b41d-abf35edc7583"]
    .Request()
    .UpdateAsync(@case);

```