---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 886da2bf000935b475cbfba040164a3fe3d28ef3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplate = await graphClient.ApplicationTemplates["{id}"]
    .Request()
    .GetAsync();

```