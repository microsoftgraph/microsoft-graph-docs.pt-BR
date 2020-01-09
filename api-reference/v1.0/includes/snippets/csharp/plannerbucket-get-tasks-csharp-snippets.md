---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fffc41c99db18e1f4205c58287b1850d6788e9e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["{task-id}"].Tasks
    .Request()
    .GetAsync();

```