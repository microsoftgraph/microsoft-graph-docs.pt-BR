---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b10feed2e8cfe1a8a11e70a3f30e420f80f4505
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationTemplate = new SynchronizationTemplate
{
    Id = "SCIM-Test1",
    ApplicationId = Guid.Parse("{id}"),
    FactoryTag = "CustomSCIM"
};

await graphClient.Applications["{id}"].Synchronization.Templates
    .Request()
    .AddAsync(synchronizationTemplate);

```