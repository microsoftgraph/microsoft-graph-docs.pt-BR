---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba0068cccad052aefb22cee907db310bde7e00ea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["gcrYAaAkgU2EQUvpkNNXLGQAGTtu"].Tasks
    .Request()
    .GetAsync();

```