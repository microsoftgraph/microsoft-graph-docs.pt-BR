---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 745f9c603862d57c1da5cfd0216e3f2d595901f0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfileStatus = await graphClient.Education.SynchronizationProfiles["{id}"].ProfileStatus
    .Request()
    .GetAsync();

```