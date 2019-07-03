---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0b07faa09a4ad952dac15b03023b4ac4feff510
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.PrivilegedRoles["{id}"].Assignments
    .Request()
    .GetAsync();

```