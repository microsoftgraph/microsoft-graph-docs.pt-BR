---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbce311abd837f04462dff26da907a2b2cdc043b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationTemplate = new SynchronizationTemplate
{
    Id = "SCIM-Test1",
    ApplicationId = "{id}",
    FactoryTag = "CustomSCIM"
};

await graphClient.Applications["{id}"].Synchronization.Templates
    .Request()
    .AddAsync(synchronizationTemplate);

```