---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 745f9c603862d57c1da5cfd0216e3f2d595901f0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611576"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfileStatus = await graphClient.Education.SynchronizationProfiles["{id}"].ProfileStatus
    .Request()
    .GetAsync();

```