---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78a46a9c67007df96ec3324b66a5a85b5d6e65b4
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Tasks
    .Request()
    .GetAsync();

```