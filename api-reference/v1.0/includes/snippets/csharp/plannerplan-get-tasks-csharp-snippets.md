---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2adb3194f88ed62d8ce501b4676efef31a21e400
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Plans["{plan-id}"].Tasks
    .Request()
    .GetAsync();

```